---
TOCTitle: Inscrição do Cliente do RMS
Title: Inscrição do Cliente do RMS
ms:assetid: '9c1d07bf-7235-4694-8291-ac2e5b221f4a'
ms:contentKeyID: 18124108
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747613(v=WS.10)'
---

Inscrição do Cliente do RMS
===========================

Os computadores clientes podem efectuar a inscrição no serviço de publicação do RMS para receber um certificado de licenciador de clientes do RMS para que os autores possam publicar conteúdo protegido pelo RMS quando os respectivos computadores não estão ligados à rede da empresa. Neste caso, o computador cliente e não o serviço de publicação assina e emite as licenças de publicação que contêm as informações dos direitos de utilização para o conteúdo protegido pelo RMS publicado a partir desse computador.

O serviço de publicação do RMS emite certificados de licenciador de clientes.

A inscrição de clientes inclui os seguintes passos:

1.  O computador cliente envia o certificado de conta de direitos do utilizador num pedido de inscrição ao serviço de publicação executado no servidor ou cluster de certificações de raiz ou num servidor ou cluster de licenciamento.
2.  O servidor valida se a inscrição do cliente é permitida com base nas definições do administrador de rede e desde que o certificado de conta de direitos não conste de uma lista de exclusões existente na base de dados de configuração. Para mais informações sobre como criar listas de exclusões, consulte "Gerir a Política de Exclusão" em "Utilizar um Servidor do RMS" nesta colecção de documentação.
3.  O serviço de publicação cria um par de chaves para o computador cliente. Cria um certificado de licenciador de clientes e coloca a chave pública no certificado. Encripta a chave privada com a chave pública do certificado de conta de direitos e, em seguida, coloca-se no certificado.
4.  O serviço de publicação emite um certificado de licenciador de clientes para o computador cliente.
