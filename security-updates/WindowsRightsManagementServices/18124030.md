---
TOCTitle: Criar a Conta de Serviço do RMS
Title: Criar a Conta de Serviço do RMS
ms:assetid: '6eb38729-f0f0-431a-bc8c-17102cf175d8'
ms:contentKeyID: 18124030
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747546(v=WS.10)'
---

Criar a Conta de Serviço do RMS
===============================

Durante a instalação, o RMS cria um grupo de segurança denominado **Grupo de Serviço do RMS** no computador local e concede-lhe as permissões adequadas para todos os recursos necessários ao funcionamento do RMS.

Quando aprovisiona o RMS num servidor, especifica uma conta de utilizador como a conta de serviço do RMS. A conta especificada torna-se num membro do Grupo de Serviço do RMS, sendo-lhe concedidas as permissões associadas a este grupo. Durante as operações normais, o RMS é executado com base na conta de serviço do RMS para a maior parte dos fins.

| ![](/security-updates/images/Cc747546.note(WS.10).gif)Nota                                  |
|--------------------------------------------------------------------------------------------------------|
| A conta de serviço do RMS não pode ser a mesma conta de domínio que foi utilizada para instalar o RMS. |

Por questões de segurança, recomenda-se a criação de uma conta especial de utilizador que deve ser utilizada como conta de serviço do RMS e nunca para nenhum outro fim. Não devem também ser concedidas outras permissões a esta conta.

| ![](/security-updates/images/Cc747546.Important(WS.10).gif)Importante |
|----------------------------------------------------------------------------------|
| Crie esta conta de utilizador especial antes de instalar e aprovisionar o RMS.   |

Para mais informações sobre as permissões concedidas ao Grupo de Serviço do RMS e sobre as contas de execução do RMS, consulte "Modelo de Segurança do RMS" na "Referência Técnica do RMS" nesta colecção de documentação.
