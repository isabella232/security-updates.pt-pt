---
TOCTitle: Planear a Implementação nas Florestas
Title: Planear a Implementação nas Florestas
ms:assetid: '2dfb40b7-95b1-4362-b32e-72867544b705'
ms:contentKeyID: 18123968
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720233(v=WS.10)'
---

Planear a Implementação nas Florestas
=====================================

Se estiver a implementar o RMS num ambiente com múltiplas florestas, tem de determinar o suporte necessário para os utilizadores e grupos externos à floresta na qual o RMS foi implementado. O problema reside no facto de, normalmente, os objectos de utilizador ou de grupo de outras florestas não terem objectos representativos na floresta onde o RMS reside. Se pretender utilizar o RMS para restringir permissões para utilizadores ou grupos de outras florestas, tem de configurar a floresta adequadamente para permitir a expansão de grupos nas florestas.

Existem duas formas de implementar o suporte de expansão de grupos em florestas para o RMS:

-   Implemente o RMS na floresta onde os grupos estão definidos e onde será utilizado para expandir os membros desses grupos.
-   Sincronize as definições de grupo nas florestas para que a instalação local do RMS determine os membros de grupo para qualquer utilizador. Se o utilizador que pede uma licença de utilização tiver uma conta do Windows numa floresta separada, tem de existir também um objecto de contacto na floresta local que represente o membro de grupo desse utilizador. Pode utilizar metadirectórios, como o Microsoft® Identity Integration Server (MIIS) 2003 ou o Identity Integration Feature Pack (IIFP), para implementar a sincronização de fidelidade total dos objectos de grupo nas florestas.

Pode planear utilizar o RMS apenas para uma floresta e pode optimizar o processo de emissão de licenças de utilização modificando a política de cluster **MaxCrossForestCalls** na base de dados de configuração do RMS. Esta política especifica o número máximo de vezes que um membro de um grupo pode passar os limites da floresta. O valor predefinido é 10. Para alterar o valor para 0, utilize o seguinte comando SQL:

`update DRMS_ClusterPolicies set PolicyData=0 em que PolicyName='MaxCrossForestCalls'`
