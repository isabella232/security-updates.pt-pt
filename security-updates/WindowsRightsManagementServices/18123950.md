---
TOCTitle: Licenças de Publicação
Title: Licenças de Publicação
ms:assetid: '187228fc-370b-4e23-a53a-21bb296b84a1'
ms:contentKeyID: 18123950
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720211(v=WS.10)'
---

Licenças de Publicação
======================

Os utilizadores de aplicações activadas pelo RMS podem atribuir direitos de utilização específicos a ficheiros digitais e informações que correspondam às políticas empresariais existentes. Estes direitos de utilização são armazenados nas licenças de publicação que especificam os utilizadores que podem ver o conteúdo e indicam a forma de edição e distribuição do conteúdo.

Uma licença de publicação pode ser emitida por uma aplicação cliente activada pelo RMS, pelo servidor de certificações de raiz ou por um servidor de licenciamento do RMS. Quando uma licença de publicação é emitida por uma aplicação cliente activada pelo RMS, um certificado licenciador de clientes é concedido à aplicação pelo servidor do RMS. Tal denomina-se publicação offline. É um método comum de publicação pois permite aos utilizadores de aplicações activadas pelo RMS criarem conteúdo protegido sem necessitarem de uma ligação a um servidor do RMS. Se a aplicação cliente activada pelo RMS não utilizar um certificado de licenciador de clientes, o utilizador tem de ligar-se a um servidor do RMS para receber uma licença de publicação para o conteúdo protegido.

Uma licença de publicação contém a chave de conteúdo simétrica para desencriptação do conteúdo encriptado com a chave pública do servidor do RMS. Isto garante que só o servidor possa desencriptar o conteúdo e emitir licenças de utilização.

Uma licença de publicação é assinada pela chave privada do servidor emissor ou pela chave privada do certificado de licenciador de clientes.
