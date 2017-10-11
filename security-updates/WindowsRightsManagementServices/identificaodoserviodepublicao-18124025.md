---
TOCTitle: Identificação do Serviço de Publicação
Title: Identificação do Serviço de Publicação
ms:assetid: '5d500841-a202-4865-b5d2-d0775d4e1bbc'
ms:contentKeyID: 18124025
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747580(v=WS.10)'
---

Identificação do Serviço de Publicação
======================================

O serviço de publicação do RMS emite licenças de publicação utilizadas na protecção do conteúdo. Também emite certificados de licenciadores de clientes que permitem aos utilizadores publicar conteúdo quando não estão ligados à rede da empresa.

O serviço de publicação está disponível a partir do cluster de certificações de raiz ou de servidores de licenciamentos. Uma aplicação activada pelo RMS pede este serviço quando um autor publica conteúdo protegido pelo RMS. Para efectuar um pedido de serviço de publicação, a aplicação obtém primeiro junto do Active Directory o URL do directório virtual Licensing do servidor no qual se localiza o serviço de publicação. Em seguida, anexa o caminho para o serviço de publicação.

Por exemplo, o URL do directório virtual Licensing de um servidor é armazenado no Active Directory da seguinte forma:

http://*nome\_servidor*/\_wmcs/Licensing

Quando um servidor pede uma licença de publicação, ele anexa o nome do ficheiro do serviço de publicação ao URL, da seguinte forma:

http://*nome\_servidor*/\_wmcs/Licensing/Publish.asmx

Se o RMS detectar que o certificado de conta de direitos se baseia na autenticação de utilizador do Windows, a localização do serviço de publicação é determinada pela floresta do Active Directory. Isto aplica-se tanto a utilizadores internos como externos que se ligam à rede da empresa através de uma rede privada virtual (VPN).

Se o RMS detectar que o certificado de conta de direitos se baseia no Microsoft® .NET Passport, a localização do serviço de publicação é a conta .NET Passport especificada no conteúdo protegido pelo RMS.

| ![](images/Cc747580.note(WS.10).gif)Nota                    |
|------------------------------------------------------------------------------------------|
| Se activou o SSL no servidor do RMS, estes URL utilizam o protocolo de ligação https://. |
