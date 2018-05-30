---
TOCTitle: Procedimentos de Administração Recomendados do RMS
Title: Procedimentos de Administração Recomendados do RMS
ms:assetid: '385f8112-da00-417f-a2b8-42dc1e06b717'
ms:contentKeyID: 18123976
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720245(v=WS.10)'
---

Procedimentos de Administração Recomendados do RMS
==================================================

Considere os seguintes procedimentos de administração recomendados para o RMS.

-   **Não Implementar Serviços Adicionais nos Servidores do RMS**
    Se executar outros serviços além dos serviços do RMS nos servidores, podem ocorrer conflitos que resultam em problemas de segurança. Utilize os contadores de desempenho para analisar a degradação ou os conflitos do serviço.
-   **Efectuar Cópias de Segurança Frequentes das Bases de Dados de Configuração**
    As bases de dados de configuração armazenam informações vitais ao funcionamento do RMS. Além disso, a base de dados de configuração do cluster de certificações de raiz contém os pares de chaves de toda a instalação. Se efectuar cópias de segurança regulares, pode restaurar rapidamente o RMS para um estado de funcionamento correcto caso um servidor de bases de dados falhe. Para além de efectuar cópias de segurança regulares, deve também testar a validade destas cópias de segurança efectuando restauros de teste (num ambiente de teste separado). Para mais informações, consulte "Efectuar Cópias de Segurança e Restaurar o Sistema para o RMS" na secção "Planear uma Implementação do RMS" nesta colecção de documentação.
-   **Optimizar Regularmente a Base de Dados de Registo**
-   **Utilizar o Microsoft Operations Manager (MOM) para Controlar o Servidor do RMS**
    Utilize o MOM e o Pacote RMS MOM para detectar eventos críticos ou a degradação do desempenho e enviar notificações sobre estes eventos.
