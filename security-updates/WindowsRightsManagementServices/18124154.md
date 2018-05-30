---
TOCTitle: Identificação do Serviço de Inscrição
Title: Identificação do Serviço de Inscrição
ms:assetid: 'bbeb00bd-04e0-4df6-8615-76aa8125b620'
ms:contentKeyID: 18124154
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747737(v=WS.10)'
---

Identificação do Serviço de Inscrição
=====================================

O primeiro servidor do RMS a ser aprovisionado na floresta tem de estabelecer ligação ao Serviço de Inscrição da Microsoft para inscrever e obter o certificado de licenciador de servidores. Para adquirir o URL para o Serviço de Inscrição, o programa de configuração do RMS efectua um pedido UDDI ao [Web site UDDI da Microsoft](http://go.microsoft.com/fwlink/?linkid=14794) (http://go.microsoft.com/fwlink/?LinkId=14794). Os servidores seguintes que são aprovisionados como parte do cluster de certificações de raiz não necessitam de obter certificados de licenciadores de servidores, uma vez que partilham a configuração do primeiro servidor de certificações de raiz.
