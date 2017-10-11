---
TOCTitle: Proteger os Servidores do RMS
Title: Proteger os Servidores do RMS
ms:assetid: '7e6c4d3a-6cfb-4e96-9dda-ead83f961a6e'
ms:contentKeyID: 18124073
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747574(v=WS.10)'
---

Proteger os Servidores do RMS
=============================

Pode seguir as seguintes recomendações para gerir as contas de utilizador e as definições de segurança dos servidores do RMS:

-   Os directórios virtuais do Web site que utiliza para administrar o RMS têm listas de controlo de acesso discricionário (DACL) que limitam o acesso aos administradores locais. Um administrador local pode criar um grupo de segurança adicional para, através da adição e remoção de membros e pela configuração de entradas de controlo de acesso (ACEs) adicionais nas páginas Web de administração, aumentar o controlo do acesso.
-   Para uma maior segurança, altere as definições da DACL na página Web Definições de Segurança (AdminSvc.asmx). Para permitir o aprovisionamento, o ACE predefinido concede controlo total à conta que aprovisiona o RMS. Após o aprovisionamento, deverá alterar o ACE para um indivíduo ou um grupo de segurança restrita.
-   Para além das permissões e direitos para cada um dos servidores do RMS, dê uma atenção especial aos requisitos de protecção da base de dados de configuração, vital para a protecção da totalidade da implementação. Para mais informações, consulte "[Proteger a Base de Dados de Configuração](https://technet.microsoft.com/e023b96f-81d0-45fb-8cc5-becaf6d47ae1)" posteriormente nesta secção.

Para mais informações sobre como proteger o Microsoft SQL Server™, consulte a página Web **SQL Server Security** no [Web site da Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).

Para mais informações sobre como proteger os computadores que estão a executar um membro da família de sistemas operativos Microsoft Windows Server 2003, transfira o "Windows Server 2003 Security Guide" a partir do Centro de Transferências da Microsoft no [Web site da Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).
