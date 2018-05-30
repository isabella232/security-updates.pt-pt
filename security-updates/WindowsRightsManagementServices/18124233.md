---
TOCTitle: Alterar a Conta de Serviço do RMS
Title: Alterar a Conta de Serviço do RMS
ms:assetid: 'f257d66d-b823-41e4-bcb7-7c90eb295238'
ms:contentKeyID: 18124233
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747736(v=WS.10)'
---

Alterar a Conta de Serviço do RMS
=================================

Durante a instalação, o RMS cria o RMS Service Group no computador local e concede-lhe as permissões adequadas relativamente a todos os recursos necessários ao funcionamento do RMS. Quando aprovisionar o RMS num servidor, a conta de serviço do RMS é definida através de uma conta de domínio. A conta de serviço do RMS não pode ser a mesma conta de domínio que foi utilizada para instalar o RMS. Essa conta torna-se membro do RMS Service Group e são-lhe concedidas as permissões associadas a este grupo. Durante as operações de rotina, o RMS opera sob a conta de serviço do RMS.

Pode alterar a conta de serviço do RMS a qualquer momento. Quando a conta é alterada, a conta anteriormente especificada é removida do RMS Service Group de forma automática, e a nova conta torna-se membro do grupo.

| ![](/security-updates/images/Cc747736.Important(WS.10).gif)Importante                                                                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Por questões de segurança, é altamente recomendável criar uma conta especial de utilizador para utilizar como conta de serviço do RMS, a qual não será utilizada para mais nenhum outro fim senão o de conta de serviço do RMS. Além disso, não deverá conceder a esta conta mais nenhuma permissão. |

| ![](/security-updates/images/Cc747736.note(WS.10).gif)Nota                                                        |
|------------------------------------------------------------------------------------------------------------------------------|
| A conta de serviço do RMS não pode ser a mesma conta de domínio que foi utilizada para instalar o RMS com o Service Pack  1. |
