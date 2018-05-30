---
TOCTitle: Identificação do Serviço de Certificação de Contas
Title: Identificação do Serviço de Certificação de Contas
ms:assetid: '293a2f91-4712-45ec-8b74-7533f4144cbd'
ms:contentKeyID: 18123919
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720224(v=WS.10)'
---

Identificação do Serviço de Certificação de Contas
==================================================

O serviço de Certificação de Contas do RMS concede certificados de conta de direitos aos utilizadores. Cada certificado de conta de direitos (RAC) só é válido para um computador ou dispositivo específico e requer que o utilizador que pede o certificado tenha um certificado de computador válido.

Só o servidor ou o cluster de certificações de raiz executa o serviço de certificação de contas. Para efectuar um pedido de certificação de conta, um cliente obtém primeiro junto do Active Directory o URL para o directório virtual Certification do servidor de certificações de raiz no qual o serviço de certificação de contas está localizado. Em seguida, anexa o caminho para o serviço de certificação de contas.

Por exemplo, O URL de Certification do servidor de certificações de raiz está armazenado no Active Directory da seguinte forma:

http://*nome\_servidor*/\_wmcs/Certification

Quando um cliente pede um certificado de conta de direitos, anexa o nome do ficheiro do serviço de certificação de conta ao URL, da seguinte forma:

http://*nome\_servidor*/\_wmcs/Certification/Certification.asmx

| ![](/security-updates/images/Cc720224.note(WS.10).gif)Nota                    |
|------------------------------------------------------------------------------------------|
| Se activou o SSL no servidor do RMS, estes URL utilizam o protocolo de ligação https://. |
