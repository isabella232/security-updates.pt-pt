---
TOCTitle: Efectuar Cópia de Segurança e Restaurar Modelos de Política de Direitos
Title: Efectuar Cópia de Segurança e Restaurar Modelos de Política de Direitos
ms:assetid: 'a6ed3328-4128-45e8-9236-3de484b460de'
ms:contentKeyID: 18124139
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747625(v=WS.10)'
---

Efectuar Cópia de Segurança e Restaurar Modelos de Política de Direitos
=======================================================================

Para proteger modelos de política de direitos valiosos, efectue regularmente uma cópia de segurança dos dados do modelo que se encontra na base de dados de configuração num suporte, e coloque-o num local seguro. Se ocorrer uma falha de sistema, os modelos de política de segurança podem ser restaurados a partir dessa cópia de segurança.

Proceda de uma das seguintes formas:

-   Efectue a cópia de segurança completa da base de dados de configuração que inclui os dados do modelo de política de direitos. Para mais informações sobre como efectuar cópias de segurança de uma base de dados do SQL Server, consulte a documentação do SQL Server.
    - ou -
-   Efectue apenas a cópia de segurança dos dados do modelo de política de direitos que se encontra na base de dados de configuração. Para tal, exporte as informações de GUID e de TemplateData da tabela DRMS\_RightsTemplate para um novo ficheiro de texto. Para mais informações sobre como exportar dados de uma base de dados do SQL Server, consulte a documentação do SQL Server.

Se tiver de restaurar os dados do modelo de política de direitos que se encontram na base de dados de configuração, pode extrair as informações de GUID e de TemplateData da tabela DRMS\_RightsTemplate da cópia de segurança da base de dados de configuração, ou então importar simplesmente os dados a partir do ficheiro de texto. Para mais informações acerca da realização destas tarefas, consulte a documentação do SQL Server.

| ![](/security-updates/images/Cc747625.note(WS.10).gif)Nota                                                                |
|--------------------------------------------------------------------------------------------------------------------------------------|
| Para definir um plano de execução de cópias de segurança de modelos de política de direitos, consulte o administrador do SQL Server. |
