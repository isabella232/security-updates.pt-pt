---
TOCTitle: Identificação do Serviço de Activação
Title: Identificação do Serviço de Activação
ms:assetid: 'e178d81b-b35c-4958-87ef-e077e2204b32'
ms:contentKeyID: 18124200
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747697(v=WS.10)'
---

Identificação do Serviço de Activação
=====================================

O serviço de activação emite cofres e certificados de computador de RMS para os clientes do RMS versão 1.0. É suportado para garantir a compatibilidade com o RMS versão 1.0. O cluster de certificações de raiz do RMS fornece o serviço de proxy de activação que reencaminha os pedidos de activação de computador do RMS para o serviço de activação dos computadores clientes executados na rede da empresa.

Para efectuar um pedido de activação de computador do RMS, um cliente do RMS versão 1.0 obtém primeiro junto do Active Directory o URL do directório virtual Certification do servidor de certificações de raiz onde o serviço de proxy de activação está localizado. Em seguida, anexa o caminho para o serviço proxy de activação.

Por exemplo, o URL para o directório virtual Certification no servidor de certificações de raiz está armazenado no Active Directory na seguinte forma:

http://*nome\_servidor*/\_wmcs/Certification

Quando um cliente pede a activação de computador do RMS, anexa o nome de ficheiro do serviço de proxy de activação ao URL, da seguinte forma:

http://*nome\_servidor*/\_wmcs/Certification/Activation.asmx

Os clientes executados fora da rede de empresa utilizam a identificação de serviço para localizarem o serviço de activação. Para mais informações, consulte "[Publicação de Serviços Alojados na Microsoft](https://technet.microsoft.com/7ee8cb4d-1b46-48be-8a4c-5ff6a458231a)" anteriormente nesta secção.

| ![](images/Cc747697.note(WS.10).gif)Nota                    |
|------------------------------------------------------------------------------------------|
| Se activou o SSL no servidor do RMS, estes URL utilizam o protocolo de ligação https://. |
