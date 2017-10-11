---
TOCTitle: Certificação de Contas do RMS
Title: Certificação de Contas do RMS
ms:assetid: 'c9a385c5-6dbb-47f5-a80f-69718e6f9deb'
ms:contentKeyID: 18124156
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747750(v=WS.10)'
---

Certificação de Contas do RMS
=============================

O processo de certificação de contas cria um certificado de conta de direitos que associa uma conta de utilizador a um computador específico e permite ao utilizador consumir conteúdo protegido pelo RMS a partir desse computador. Quando o utilizador publica pela primeira vez conteúdo protegido pelo RMS ou tenta consumir conteúdo protegido pelo RMS a partir de um computador cliente, a aplicação activada pelo RMS envia um pedido de certificado de conta de direitos ao serviço de certificação de contas do RMS.

O serviço de certificação pode autenticar o utilizador através da autenticação do Windows ou de um certificado x.509 armazenado no dispositivo de encriptação de hardware, tal como um smart card. Após a autenticação do utilizador, o servidor do RMS cria um certificado de conta de direitos para o utilizador com base nas respectivas credenciais autenticadas. Encripta a chave privada do utilizador com a chave pública do computador cliente do certificado de computador do RMS e inclui a chave encriptada no certificado de conta de direitos. Em seguida, emite o certificado de conta de direitos para a aplicação que efectuou o pedido, armazenando o certificado de conta de direitos no computador ou dispositivo para o disponibilizar para pedidos de licença de publicação ou de utilização subsequentes. O certificado de conta de direitos é também armazenado na base de dados de configuração.

A certificação de contas segue o processo de activação pois o certificado de computador do RMS para o computador cliente tem de pedir o certificado de conta de direitos.

Os utilizadores têm de adquirir um certificado de conta de direitos para cada computador utilizado. Se um utilizador trabalhar em mais de um computador, é emitido um certificado de conta de direitos para cada computador. No entanto, todos os computadores contêm o mesmo par de chaves para esse utilizador.

Quando uma aplicação activada pelo RMS pede uma licença de utilização, inclui o certificado de conta de direitos no pedido. O serviço de licenciamento utiliza a chave pública do certificado de conta de direitos para encriptar a chave de conteúdo. Isto garante que apenas o utilizador autenticado pode utilizar a licença de utilização.

O processo de certificação de contas envolve os seguintes passos:

1.  Quando o utilizador publica pela primeira vez conteúdo protegido pelo RMS ou tenta consumir conteúdo protegido pelo RMS num computador específico, a aplicação activada pelo RMS envia um pedido de certificado de conta de direitos ao serviço de certificação de contas executado no servidor de certificações de raiz.
2.  O serviço de autenticação de contas autentica o utilizador utilizando a autenticação do Windows.
3.  O serviço de certificação de contas cria um certificado de conta de direitos para o utilizador com base nas respectivas credenciais autenticadas. Encripta a chave privada do utilizador com a chave pública do certificado de computador do RMS e inclui a chave encriptada no certificado. Em seguida, emite o certificado de conta de direitos para a aplicação que efectuou o pedido.
4.  A aplicação armazena o certificado de conta de direitos no computador ou dispositivo para o disponibilizar para pedidos de licença de publicação ou de utilização subsequentes.

O serviço de certificação de contas utilizado pelo cliente para pedir o RAC depende do tipo de computador onde o cliente do RMS foi instalado. Os computadores de secretária padrão ligam ao serviço de certificação de contas (certification.asmx). Os serviços de servidor activados para serem utilizados com o RMS SP1 recebem os RAC a partir do serviço de certificação de servidores (ServeCertfication.asmx). Os dispositivos móveis activados para serem utilizados com o RMS SP1 recebem os RAC a partir do serviço de certificação de dispositivos móveis (MobileDeviceCertfication.asmx). Apenas o serviço de certificação de contas é activado numa instalação predefinida do RMS SP1.

Para mais informações sobre a utilização do RMS SP1 com serviços de dispositivos móveis e de servidores, consulte "Activar o Suporte do Servidor do RMS para Serviços de Dispositivos Móveis e de Servidores" em Utilizar um Servidor do RMS nesta colecção de documentação.
