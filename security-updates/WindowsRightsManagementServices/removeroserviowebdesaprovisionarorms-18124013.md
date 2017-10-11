---
TOCTitle: 'Remover o Serviço Web (Desaprovisionar o RMS)'
Title: 'Remover o Serviço Web (Desaprovisionar o RMS)'
ms:assetid: '68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e'
ms:contentKeyID: 18124013
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747602(v=WS.10)'
---

Remover o Serviço Web (Desaprovisionar o RMS)
=============================================

Depois de o servidor do RMS ter sido desactivado e toda a protecção do RMS ter sido removida, pode remover o serviço Web através dos seguintes passos:

-   Na página **Administração Global**, seleccione **Remover o RMS deste Web site**.

Apesar de em qualquer situação o RMS ser removido do IIS, o passo seguinte depende do tipo de servidor que está a ser removido.

-   Se o servidor estiver integrado num cluster (e não for o último servidor do cluster), não são necessários passos adicionais.
-   Se o servidor for apenas um servidor de licenciamento, remova a base de dados dos serviços de directório mas mantenha a base de dados de configuração e de registo (são utilizados pelo servidor de certificação que ainda está a funcionar).
-   Se o servidor for o último servidor do RMS existente na organização, mantenha a base de dados de configuração e de registo, mas remova o ponto de ligação de serviço (SCP) do Active Directory.
