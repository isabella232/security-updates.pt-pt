---
TOCTitle: Segurança Durante a Utilização Normal do RMS
Title: Segurança Durante a Utilização Normal do RMS
ms:assetid: '98f3d584-6320-4aa1-9959-7133cfdb6df7'
ms:contentKeyID: 18124106
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747609(v=WS.10)'
---

Segurança Durante a Utilização Normal do RMS
============================================

Depois de instalar e aprovisionar o RMS, os serviços Web do RMS funcionam como aplicações do IIS, acedendo a diversos recursos do sistema que requerem autenticação e autorização. Todos os recursos do sistema necessitam de ser autenticados. Caso contrário, não podem ser configurados. Esta página descreve a estrutura de autorização do RMS.

Os serviços Web do RMS são executados no contexto de um grupo de aplicações do IIS. Cada grupo de aplicações no IIS tem uma identificação exclusiva que pode corresponder a uma conta de utilizador de domínio, a uma conta de utilizador local, à conta local do Serviço de Rede ou à conta local do Sistema Local. Cada uma destas contas tem diferentes graus de autorização no sistema. Quando o RMS é aprovisionado, pode optar por executar os serviços Web do RMS como conta de Sistema Local ou como conta de utilizador de domínio. Esta conta torna-se na identidade de grupo de aplicação para o grupo de aplicações do RMS. O grupo de aplicações para o Web site da Administração Global é o "DRMS Application Pool". O grupo de aplicações para o Web site que aprovisiona chama-se "\_DRMSAppPool1". O Serviço de Registo do RMS é executado como um serviço separado do Windows na mesma conta como especificado para a identidade do grupo de aplicações do RMS.

Os recursos de que os serviços Web do RMS necessitam para o acesso incluem diversos ficheiros e pastas do sistema, bases de dados e procedimentos armazenados no servidor de bases de dados, o registo local, o Active Directory, a cache de assemblagem, a memória e outros processos executados no sistema. O Serviço de Registo do RMS necessita também de acesso à fila de mensagens de registo do sistema local. Cada um desses recursos tem os seus próprios DACLs que definem quem está autorizado a aceder ao recurso e de que forma pode ser utilizado. 

Para simplificar a atribuição de permissões e a gestão de contas do serviço, todas as permissões necessárias são atribuídas ao RMS Service Group local que o RMS criou durante o aprovisionamento. Como a conta de serviço do RMS é um membro deste grupo, recebe todas as permissões atribuídas ao grupo.

A lista seguinte apresenta um resumo das permissões que foram concedidas ao RMS Service Group:

-   Permissão de Leitura para os directórios de raiz virtual
-   Permissões de Escrita para o directório da cache de assemblagem
-   Permissão de Escrita para o directório temporário do sistema
-   Permissão de Escrita para a fila de registo
-   Permissão de Leitura para o Active Directory

Se estiver a utilizar o Microsoft SQL Server 2000 como o servidor de bases de dados, lembre-se de que é utilizado um método de atribuição de permissões ligeiramente diferente do aplicado pelo Windows Server 2003. O aprovisionamento do RMS cria um início de sessão para a conta de serviço do RMS no SQL Server. Se optou por aprovisionar o RMS utilizando a conta de Sistema Local, o início de sessão do SQL Server é criado com o formato *DOMÍNIO\\nome\_computador*, em que *DOMÍNIO* é o nome do domínio do Active Directory no qual o computador é membro e *nome\_computador* é o nome do servidor. Uma função SQL denominada rms\_service é criada, sendo-lhe atribuídas todas as permissões necessárias. O início de sessão para a conta de serviço do RMS é adicionado a este grupo. Nenhuma permissão é concedida explicitamente à conta de serviço do RMS.

Adicionalmente, o SQL Server atribui um proprietário de base de dados (DBO) a cada base de dados. A propriedade de base de dados é atribuída da seguinte forma durante o aprovisionamento:

-   O DBO da base de dados de Configuração é atribuído à conta de domínio utilizada no aprovisionamento do RMS.
-   O DBO das bases de dados de Serviços de Directório e de Registo é atribuído à conta de serviço do RMS.

As permissões de todos os recursos criados pelo RMS são cuidadosamente seleccionadas durante a estruturação do RMS em função da segurança. Em princípio, para nenhum dos recursos deverá ser necessário modificar as permissões que são atribuídas durante o aprovisionamento. Se tiver de alterar a conta ou a palavra-passe de utilizador para a conta de serviço após o aprovisionamento, utilize a página Administração Global do RMS. Para mais informações, consulte "Para Alterar a Palavra-passe da Conta de Serviço do RMS" em "Utilizar um Servidor do RMS" nesta colecção de documentação.
