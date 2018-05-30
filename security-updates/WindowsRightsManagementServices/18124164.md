---
TOCTitle: Eliminar Contas de Utilizadores
Title: Eliminar Contas de Utilizadores
ms:assetid: 'bf73b141-d4d1-4807-a773-3aaff58b0db6'
ms:contentKeyID: 18124164
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747653(v=WS.10)'
---

Eliminar Contas de Utilizadores
===============================

Quando uma conta de utilizador é eliminada do Active Directory, a entrada do certificado de conta de direitos desse utilizador que se encontra na tabela de chaves de utilizador da base de dados de configuração do cluster de configurações de raiz não é eliminada automaticamente. Por este motivo, a tabela de chaves de utilizador pode crescer ilimitadamente à medida que vão sendo adicionadas novas chaves de utilizador, sem que as antigas sejam eliminadas.

Para efectuar a manutenção da base de dados de configuração, é possível executar um procedimento que elimina uma chave de utilizador através do respectivo identificador de segurança (SID) sempre que a conta de utilizador associada é retirada do Active Directory. Como alternativa, pode também executar periodicamente um script que elimine da base de dados de configuração as chaves de utilizador que estejam associadas a SIDs que já não existem no Active Directory. Convém referir que este procedimento origina uma carga muito grande tanto no SQL Server como no Active Directory.
