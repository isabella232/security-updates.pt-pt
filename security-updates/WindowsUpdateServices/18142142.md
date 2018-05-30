---
TOCTitle: 'Documento Leia-me do Windows Server Update Services'
Title: 'Documento Leia-me do Windows Server Update Services'
ms:assetid: '4244109a-395a-4ff8-9989-ea55ab0964a3'
ms:contentKeyID: 18142142
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720505(v=WS.10)'
---

Documento Leia-me do Windows Server Update Services
===================================================

Este documento descreve questões conhecidas que afectam o Windows Server Update Services (WSUS). Inclui recomendações e requisitos de instalação para o WSUS.

| ![](/security-updates/images/Cc720505.note(WS.10).gif)Nota                                                                                                                                                                         |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Existe uma cópia deste documento disponível para transferência no Centro de Transferências da Microsoft, em [http://go.microsoft.com/fwlink/?LinkId=48126](http://go.microsoft.com/fwlink/?linkid=48126). Esta página poderá estar em inglês. |

Antes de começar
----------------

#### Ponto 1: O IIS tem de estar instalado

O Microsoft® Windows Server™ Update Services (WSUS) requer que o componente Serviços de Informação Internet (IIS, Internet Information Services) esteja instalado. No entanto, no Microsoft Windows Server 2003 e no Microsoft Windows® 2000 Server, o IIS não está instalado por predefinição. Por conseguinte, é possível que o Programa de Configuração do Windows Server Update Services não consiga continuar, apresentando uma mensagem de erro a indicar que o IIS não está instalado.

Para instalar o IIS:

1.  Abra o Painel de Controlo.
2.  Faça duplo clique em **Adicionar ou Remover Programas**.
3.  Clique em **Adicionar/Remover Componentes do Windows**.
4.  Na lista **Componentes**, clique em **Servidor de Aplicações**.
5.  Clique em **Detalhes**.
6.  Seleccione a caixa de verificação **ASP.NET**. Active o **acesso COM+ à rede** e o componente Serviços de Informação Internet (IIS) será seleccionado automaticamente.
7.  Seleccione **Serviços de informação Internet (IIS)** e clique em **Detalhes** para ver a lista de componentes opcionais do IIS.
8.  Seleccione todos os componentes opcionais que pretende instalar. O componente opcional Serviço World Wide Web inclui subcomponentes importantes, tais como o componente Active Server Pages e a ferramenta de Administração Remota (HTML). Para ver e seleccionar estes subcomponentes, clique em Serviço World Wide Web e, em seguida, clique em Detalhes. Clique em OK até regressar ao Assistente de Componentes do Windows.
9.  Clique em **Seguinte** e conclua o Assistente de Componentes do Windows.
10. Após instalar o IIS, execute o Programa de Configuração do Windows Server Update Services.

#### Ponto 2: Para servidores com o Windows 2000 Server, é necessário que pelo menos um Web site esteja presente no IIS antes da instalação do WSUS

O Programa de Configuração do Windows Server Update Services poderá não conseguir criar um Web site, caso não estivessem presentes sites no IIS aquando da execução do Programa de Configuração. Tal poderá ocorrer, por exemplo, se tiver um site do Software Update Services (SUS) 1.0 como único site no IIS e o eliminar antes de instalar o WSUS.

Neste caso, será necessário criar um novo Web site utilizando o snap-in Gestor dos Serviços de Informação Internet (IIS). Em seguida, poderá seleccionar este site ou especificar um novo site durante a configuração do WSUS.

Se já tiver tentado instalar o WSUS e tiver ocorrido uma falha no Programa de Configuração por não haver sites presentes, abra o snap-in Gestor do IIS e elimine o site "Web Site 1". Em seguida, siga os passos descritos anteriormente e execute novamente o Programa de Configuração.

#### Ponto 3: Instalar componentes de pré-requisitos

#### Requisitos de software

A tabela abaixo mostra o software necessário para cada sistema operativo suportado. Antes de executar o Programa de Configuração do WSUS, certifique-se de que o servidor WSUS preenche esta lista de requisitos. Se alguma destas actualizações exigir que o computador seja reiniciado quando a instalação estiver concluída, deverá reiniciar antes de instalar o WSUS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Sistema operativo</th>
<th style="border:1px solid black;" >Requisitos</th>
<th style="border:1px solid black;" >Transferências</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Todos os sistemas operativos</td>
<td style="border:1px solid black;">Serviços de Informação Internet da Microsoft (IIS) 5.0</td>
<td style="border:1px solid black;">Instalar a partir do sistema operativo.
Consulte o ponto 1: O IIS tem de estar instalado.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Todos os sistemas operativos</td>
<td style="border:1px solid black;">BITS (Background Intelligent Transfer Service) 2.0</td>
<td style="border:1px solid black;">Para sistemas operativos Windows Server 2003, consulte a <a href="http://go.microsoft.com/fwlink/?linkid=47251">Actualização para Background Intelligent Transfer Service (BITS) 2.0 e WinHTTP 5.1 Windows Server 2003</a> (KB842773), no Centro de Transferências (http://go.microsoft.com/fwlink/?LinkId=47251).
Para sistemas operativos Windows Server 2000, consulte a <a href="http://go.microsoft.com/fwlink/?linkid=46794">Actualização para Background Intelligent Transfer Service (BITS) 2.0 e WinHTTP 5.1 Windows 2000</a> (KB842773), no Centro de Transferências (http://go.microsoft.com/fwlink/?LinkId=46794).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1 para Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Microsoft .NET Framework 1.1 Service Pack 1 para Windows Server 2003</a>
Em alternativa, consulte o <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> e procure Actualizações de Alta Prioridade e Service Packs; instale o Microsoft .NET Framework 1.1 Service Pack 1 para Windows Server 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Software de base de dados 100% compatível com o Microsoft SQL</td>
<td style="border:1px solid black;">N/D</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Software de base de dados 100% compatível com o Microsoft SQL</td>
<td style="border:1px solid black;">Se não estiver a utilizar o Microsoft SQL Server 2000, pode instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000). Para tal, são necessário vários passos. Para mais informações, consulte a secção sobre como Instalar o MSDE no Windows 2000, mais abaixo.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft Internet Explorer 6.0 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework Version 1.1 Redistributable Package</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework Version 1.1 Redistributable Package</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a>
Em alternativa, consulte o <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> e procure Actualizações de Alta Prioridade e Service Packs; instale o Microsoft .NET Framework 1.1 Service Pack 1 para Windows Server 2000.</td>
</tr>
</tbody>
</table>
 

Além destes requisitos, o WSUS poderá instalar ou configurar a versão 1.1 do ASP.NET no servidor, caso seja necessário. (O Programa de Configuração do WSUS configura o ASP.NET.)

#### Instalar o MSDE 2000 no Windows 2000

Se estiver a utilizar o Windows 2000 para o WSUS e não tiver acesso ao Microsoft SQL Server 2000, deverá instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE) antes de executar o Programa de Configuração do WSUS. Se já tiver o MSDE instalado no servidor WSUS, não será necessário configurar uma instância especial do mesmo para o WSUS. Poderá simplesmente indicar o nome da instância existente durante o processo de configuração do WSUS.

A instalação do MSDE no Windows 2000 Server é um processo de quatro passos. Primeiro, é necessário transferir e expandir o arquivo do MSDE para uma pasta no servidor WSUS. Em seguida, utilize uma linha de comandos e opções de linha de comandos para executar o Programa de Configuração do MSDE, para definir a palavra-passe SA e para atribuir o WSUS como nome de instância. Quando a instalação do MSDE estiver concluída, deverá confirmar se a instância WSUS está a ser executada como um serviço NT. Finalmente, tem de adicionar uma actualização de segurança ao MSDE para proteger o servidor WSUS.

#### Passo 1: Transferir e expandir o arquivo do MSDE

É necessário transferir e expandir o arquivo do MSDE para uma pasta no servidor WSUS. Consulte [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Passo 2: Instalar o MSDE

Utilize uma linha de comandos e opções de linha de comandos para executar o Programa de Configuração do MSDE, para definir a palavra-passe SA e para atribuir o WSUS como nome de instância. Quando a instalação do MSDE estiver concluída, deverá confirmar se a instância WSUS está a ser executada como um serviço NT.

Para instalar o MSDE, defina a palavra-passe SA e atribua um nome de instância:

1.  Na linha de comandos, navegue para a pasta de instalação do MSDE especificada no "Passo 1: Transferir e expandir o arquivo do MSDE".
2.  Escreva o seguinte: **setup sapwd="***password***" instancename=WSUS**
    sendo que *password* é uma palavra-passe segura para a conta SA nesta instância do MSDE, e sendo que **instancename** é o nome da instância de base de dados. Em alternativa, é possível utilizar o nome de instância predefinido (em vez de "WSUS") para a base de dados WSUS. Se optar por esta alternativa, não será necessário escrever **instancename=WSUS** no parâmetro da linha de comandos. Este comando inicia o programa de configuração do MSDE, define a palavra-passe SA e atribui o nome que especificar a esta instância do MSDE.

#### Passo 3: Confirmar se a instância WSUS do MSDE está instalada

Deve certificar-se de que consegue visualizar a instância WSUS do MSDE.

1.  Clique em **Iniciar** e, em seguida, clique em **Executar**.
2.  Na caixa **Abrir**, escreva **services.msc** e, em seguida, clique em **OK**.

Percorra a lista de serviços e verifique se existe um serviço com o nome MSSQL$WSUS (caso tenha utilizado "WSUS" para o nome da instância) ou MSSQLSERVER (caso tenha utilizado o nome de instância predefinido).

#### Passo 4: Iniciar a instância do MSDE.

Quando terminar a instalação do MSDE, terá de iniciar a instância. Caso tenha utilizado "WSUS" para o nome da instância, será necessário iniciar o "MSSQL$WSUS". Caso tenha utilizado o nome de instância predefinido, será necessário iniciar o MSSQLSERVER. A menos que inicie este serviço, o WSUS não conseguirá utilizar a instância de base de dados.

#### Passo 5: Actualizar o MSDE

Tem de transferir e instalar a actualização de segurança descrita no boletim [MS03-031: Patch de segurança cumulativo para o SQL Server](http://go.microsoft.com/fwlink/?linkid=47364).

Para transferir a actualização de segurança, consulte o boletim [MS03-031 sobre o patch de segurança para o SQL Server 2000 (32 bits)](http://go.microsoft.com/fwlink/?linkid=47363).

#### Ponto 4: Requisitos mínimos de espaço em disco

Seguem-se os requisitos mínimos de espaço em disco para instalação do Windows Server Update Services:

-   1 gigabyte (GB) na partição do sistema
-   2 GB para o volume no qual os ficheiros de base de dados serão armazenados
-   6 GB, com base em cálculos de projecção de conteúdo

#### Ponto 5: Antes de instalar a versão mais recente, é necessário desinstalar versões anteriores do WSUS através da opção para Adicionar ou Remover Programas

Se planear instalar o Windows Server Update Services num servidor que tenha o Windows Update Services Beta 1 ou Beta 2 instalado, terá primeiro de desinstalar a versão anterior utilizando a opção para Adicionar ou Remover Programas, no Painel de Controlo.

#### Ponto 6: O WSUS requer que a opção de accionadores aninhados esteja activada no SQL Server

Esta opção está activada por predefinição; no entanto, pode ser desactivada por um administrador do SQL Server.

Se planear utilizar uma base de dados SQL Server como arquivo de dados do Windows Server Update Services, o administrador do SQL Server deverá confirmar se a opção de accionadores aninhados está activada antes de o administrador do WSUS instalar o WSUS e especificar a base de dados durante a configuração.

O Programa de Configuração do WSUS activa a opção RECURSIVE\_TRIGGERS, que é uma opção específica de base de dados; no entanto, não activa a opção de accionadores aninhados, que é uma opção global de servidor.

Para ver se a opção de accionadores aninhados está activada, utilize:

**sp\_configure 'nested triggers'**

Para activar a opção de accionadores aninhados no SQL Server, execute o seguinte a partir de um ficheiro batch no computador com SQL Server:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Ponto 7: Parâmetros de linha de comandos do Programa de Configuração do WSUS

É possível efectuar instalações automáticas do WSUS. Para mais informações e para obter os parâmetros da linha de comandos, consulte o Anexo A sobre instalação automática na [Implementação do Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

Problemas conhecidos
--------------------

#### Ponto 1: IIS Lockdown Wizard

Se estiver a executar o IIS num computador com o Windows 2000 Server, instale a versão mais recente do IIS Lockdown Wizard (que inclui URLScan) a partir da página da ferramenta IIS Lockdown no Web site Microsoft TechNet. A Microsoft recomenda vivamente que instale esta ferramenta para ajudar a manter os servidores IIS seguros. O IIS Lockdown Wizard funciona desactivando funcionalidades do IIS desnecessárias, reduzindo assim a exposição ao risco de segurança.

| ![](/security-updates/images/Cc720505.note(WS.10).gif)Nota                                                                                                                                                          |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| O Programa de Configuração do WSUS não instala estes componentes. Terá de os instalar manualmente. Não é necessário instalar o IIS Lockdown em computadores com o Windows Server 2003, pois a funcionalidade está incorporada. |

#### Ponto 2: A alteração da configuração do WSUS directamente na base de dados não é suportada

O Windows Server Update Services armazena os respectivos dados de configuração numa base de dados (MSDE ou SQL Server). No entanto, a alteração dos dados de configuração acedendo-se directamente à base de dados não é suportada. Os administradores não deverão tentar modificar a configuração do WSUS desta forma. A forma suportada para alteração da configuração do WSUS consiste em utilizar a consola WSUS ou iniciar APIs do WSUS.

#### Ponto 3: O scripting activo terá de estar activado para que seja possível aceder ao site de administração do WSUS

Na estação de trabalho do administrador, o Internet Explorer terá de ser configurado para permitir scripting activo, de modo a ser possível utilizar o Internet Explorer para aceder ao site de administração do WSUS.

#### Ponto 4: O IIS será reiniciado durante a configuração do WSUS

O Programa de Configuração do Windows Server Update Services irá reiniciar o IIS sem aviso prévio. Tal poderá afectar Web sites existentes na organização.

#### Ponto 5: Alterar o acesso ao directório virtual de pontos de gestão SMS ou do WSUS

Por predefinição, o directório virtual de conteúdo do Windows Server Update Services está definido com acesso anónimo. Se alterar esta definição para requerer autenticação, os clientes receberão erros de autenticação e o respectivo acesso à transferência de actualizações será negado. Trata-se de um problema conhecido, em que o Winhttp.dll utiliza o contexto de autenticação incorrecto quando é necessária uma autenticação implícita, pelo que ocorrerá uma falha na autenticação. Para evitar este problema, certifique-se de que o servidor WSUS e os pontos de gestão SMS estão configurados com acesso anónimo a directórios virtuais do IIS.

#### Ponto 6: Ao instalar o WSUS no Windows Small Business Server 2003, é necessário modificar as definições de acesso de raízes virtuais (vroots) WSUS do Web site predefinido para permitir que os clientes WSUS se actualizem a partir do servidor

O Servidor WSUS instala duas raízes virtuais, SelfUpdate e ClientWebService, e alguns ficheiros no directório raiz do Web site predefinido (na porta 80). Tal permite que os clientes se actualizem através do Web site predefinido. Por predefinição, no Windows Small Business Server 2003, o Web site predefinido está configurado para recusar acesso a outro IP ou localhost que não os do servidor. Isto significa que é recusado acesso as raízes virtuais SelfUpdate e ClientWebService e que os clientes não se irão actualizar. Para conceder acesso aos clientes para auto-actualização, siga os passos abaixo descritos nas raízes virtuais SelfUpdate e ClientWebService do Web site predefinido.

1.  Clique em **Propriedades** da raiz virtual, depois em **Segurança de Directório**, clique em **Restrições de endereço IP e de nome de domínio** e, depois, clique em **Editar**.
2.  Seleccione **Acesso Concedido** e clique em **OK**. Feche todas as páginas de propriedades.

#### Ponto 7: Instalar o WSUS no Small Business Server - Problemas de Integração

-   Se o Windows Small Business Server 2003 utilizar um servidor proxy ISA para aceder à Internet, terá de introduzir manualmente os dados abaixo na interface de utilizador **Definições**: definições do servidor proxy, nome do servidor proxy e porta.
-   Se o ISA estiver a utilizar a Autenticação Windows, as credenciais do servidor proxy deverão ser introduzidas sob a forma "DOMÍNIO\\utilizador" (sendo que o utilizador pertence ao grupo "Utilizadores Internet").

#### Ponto 8: Ao mover um computador de um grupo de computadores para outro, poderá ser necessário aguardar uma hora até que o computador apareça no novo grupo conforme visualizado a partir da consola administrativa

Quando um computador é atribuído a um grupo de destino pela primeira vez, os dados nesse computador são modificados com as informações do grupo. Esses dados são actualizados periodicamente ou a cada hora. Por conseguinte, ao mover um computador de um grupo de computadores para outro, poderá ser necessário aguardar uma hora até que as informações sejam actualizadas no cliente e apresentadas conforme alteradas na consola administrativa do WSUS.

#### Ponto 9: Se instalar o WSUS num servidor membro e pretender depois promover esse servidor membro a controlador de domínio, deverá desinstalar primeiro o WSUS

Se instalar o WSUS num servidor membro e pretender depois promover esse servidor membro a controlador de domínio, será necessário seguir os seguintes passos:

1.  Desinstalar o WSUS.
2.  Promover o servidor a controlador de domínio.
3.  Reinstalar o WSUS.

#### Ponto 10: Se pretender despromover um servidor WSUS de controlador de domínio a servidor membro, deverá primeiro desinstalar o WSUS

Se estiver a executar o servidor WSUS num controlador de domínio e pretender despromover o controlador de domínio a servidor membro, terá de seguir os seguintes passos:

1.  Desinstalar o WSUS e manter a base de dados.
2.  Criar uma conta de utilizador denominada ASPNET.
3.  Na linha de comandos, introduza **aspnet\_regiis -i**.
4.  Reinstalar o WSUS e utilizar a base de dados mantida.

#### Ponto 11: Se o .NET Framework 1.0 ou 2.0 for instalado após a instalação do WSUS, a consola administrativa WSUS não será apresentada

Tal acontece porque o .NET Framework 1.0 é registado com o IIS e o servidor WSUS requer o .NET Framework 1.1. Para solucionar este problema, abra aspnet\_regiis.exe e execute os comandos abaixo, sendo que *website id* é o valor contido na seguinte chave de registo:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\Content

#### Ponto 12: Limitações de SQL remoto

O WSUS oferece suporte limitado para execução de software de base de dados num computador separado do computador que contém o resto da aplicação WSUS.

-   Não é possível utilizar o Windows 2000 Server como computador front-end num par de SQL remoto.
-   Não é possível utilizar um servidor configurado como controlador de domínio no front-end nem no back-end do par de SQL remoto.
-   Não é possível utilizar o WMSDE ou o MSDE para software de base de dados no computador back-end.
-   A configuração de um SQL Server remoto (para utilizar como a base de dados WSUS) falha se os Serviços de Terminal estiverem instalados no servidor remoto e a funcionar no modo de aplicações. Ao instalar o SQL Server num servidor de Serviços de Terminal, terá de fazer o seguinte:
    1.  Antes de executar o Programa de Configuração, abra uma linha de comandos e escreva: **change user /install**
    2.  Execute o Programa de Configuração do SQL Server.
    3.  Após executar o Programa de Configuração, na linha de comandos escreva: **change user /execute**
-   Deve ser um membro do grupo de segurança dos administradores locais no computador front-end e back-end para configurar a base de dados remota SQL Server do WSUS.
-   Para mais informações sobre problemas de SQL remoto, consulte o Apêndice C sobre SQL remoto na [Implementação do Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

#### Ponto 13: Um servidor de réplica a jusante poderá ter menos aprovações que o servidor principal a montante

Um servidor de réplica a jusante poderá ter menos aprovações que o servidor principal a montante. Tal sucede porque as aprovações de instalação só flúem para um servidor a jusante depois de o conteúdo acabar de ser transferido no servidor a montante.

#### Ponto 14: Se ocorrer uma falha na sincronização, tente executá-la novamente

Se a sincronização falhar, poderá obter uma mensagem de erro. Caso tal ocorra, deverá tentar primeiro a sincronização.

#### Ponto 15: Ao tentar aceder à consola de Administração do WSUS, aparece uma mensagem de erro System.IO.FileNotFoundException

Se receber a mensagem de erro seguinte, poderá ter de ajustar as permissões no Serviço de Rede ou nas contas ASP.NET:

System.IO.FileNotFoundException: o nome de ficheiro ou assemblagem *xxxxxx*.dll, ou uma das respectivas dependências, não foi encontrado

Sendo que *xxxx* é um nome aleatório.

Para solucionar este problema em sistemas operativos Windows Server 2003, conceda à conta de Serviço de Rede acesso de leitura/escrita a %systemroot%\\Temp. No Windows 2000 Server, conceda à conta ASP.NET acesso de leitura/escrita a %systemroot%\\Temp.

#### Ponto 16: Actualização de Segurança SQL MS03-031 (KB815495)

Esta actualização poderá aparecer como instalada no servidor WSUS, apesar de ter ocorrido uma falha de instalação no cliente. Como tal, é possível que o pacote seja novamente oferecido ao cliente. É possível solucionar este problema anulando a aprovação da actualização no servidor.

#### Ponto 17: As definições do IIS são perdidas durante a actualização RTM.

Se instalar o WSUS RTM num servidor com uma versão anterior do WSUS (por exemplo, RC), o WSUS RTM irá desinstalar a versão anterior e instalar em seguida a nova versão. Isto significa que as raízes virtuais e ficheiros associados ao WSUS no IIS serão eliminados.

Se tiver instalado o WSUS no Web site predefinido, irá perder todas as definições relacionadas com o WSUS que tenham sido estabelecidas para as raízes virtuais WSUS. Por exemplo, se tiver configurado as raízes virtuais WSUS para SSL de modo a proteger o WSUS, será necessário configurá-las novamente após instalar a versão RTM do WSUS. Nota: Receberá uma notificação na consola WSUS a informar que o SSL não está activado.

Se tiver instalado o WSUS noutro Web site que não o Web Site Predefinido, serão perdidas todas as definições adicionais ao nível do Web site do WSUS.

#### Ponto 18: Utilizar cabeçalhos de anfitrião

Se pretender atribuir valores de cabeçalho de anfitrião ao Web site predefinido (Web site do WSUS) no IIS, terá de adicionar “Todos Não Atribuídos” ou um endereço IP atribuído à lista de endereços IP sem valor de cabeçalho de anfitrião para o Web site predefinido. O mesmo deverá ser adicionado ao Web site não predefinido

**Aviso**: Poderá quebrar-se a funcionalidade do Windows® SharePoint® Services e Exchange.

#### Ponto 19: O URL da consola WSUS tem de ser adicionado à lista de zonas de conteúdo Web de Sites Fidedignos e Intranet Local em computadores nos quais esteja activada a protecção do Internet Explorer

Se tiver a protecção do Internet Explorer (também conhecida como componente de Configuração de Segurança Avançada do Internet Explorer no Microsoft Windows Server 2003) activada num computador e não adicionar a consola WSUS às zonas de conteúdo Web de Sites Fidedignos e Intranet Local, ser-lhe-ão pedidas credenciais de utilizador sempre que abrir uma página na consola WSUS.

Para adicionar a consola WSUS às zonas de conteúdo Web de **Intranet Local** e **Sites Fidedignos**:

1.  Abra **Opções da Internet** (por exemplo, clique em **Iniciar**, aponte para **Painel de Controlo** e clique em **Opções da Internet**).
2.  No separador **Segurança**, clique em **Intranet local**, clique em **Sites**, clique em **Avançadas**, adicione o URL (http://*nomeservidorWSUS*/WSUSAdmin) e clique em **OK**.
3.  Clique em **Sites fidedignos**, depois clique em **Sites**, adicione o URL da consola WSUS, clique em **OK** e, em seguida, clique novamente em **OK** para sair das **Opções da Internet**.

#### Ponto 20: Falha na actualização do WSUS Release Candidate

A actualização do WSUS Release Candidate poderá falhar devido a um problema na árvore de auto-actualização. Isto pode ocorrer se vários clientes procederem à auto-actualização ao mesmo tempo que os tenta actualizar.

Para resolver este problema:

1.  Desligue o servidor WSUS da rede, certificando-se de que os clientes não conseguem estabelecer ligação.
2.  Na linha de comandos, escreva: **iisrestart /reset** e prima ENTER.
3.  Execute a actualização.

#### Ponto 21: Algumas aprovações do SUS 1.0 não migram para o WSUS.

Ao migrar do SUS 1.0 para o WSUS, algumas aprovações no servidor SUS 1.0 não migram para o servidor WSUS. Isto deve-se ao facto de uma série de actualizações que estavam disponíveis para o SUS 1.0 já não se encontrarem disponíveis para o WSUS. Além disso, uma vez que o WSUS suporta mais actualizações do que o SUS, poderão existir actualizações importantes no servidor WSUS que são desaprovadas após a conclusão do processo de migração.

A Microsoft recomenda que reveja o conjunto de actualizações desaprovadas no seu servidor WSUS após a migração do SUS 1.0.

Para mais informações sobre a migração do SUS 1.0 para o WSUS, consulte o [Guia passo a passo para migrar de Software Update Services para Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=48042), em http://go.microsoft.com/fwlink/?LinkId=48042.

#### Ponto 22: Corrija esta entrada de registo antes de proceder à actualização para o WSUS 2.0 Service Pack 1, caso tenha migrado o WMSDE para o SQL Server

Caso planeie actualizar o WSUS 2.0 para o Service Pack 1 e tenha migrado a instalação WMSDE para o SQL Server (quer seja remoto ou local), certifique-se de que altera a seguinte entrada de registo:

HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled

O valor deve ser alterado de 1 para 0.

#### Ponto 23: Migrar uma instalação SQL remota para o WSUS 2.0 Service Pack 1

Siga os seguintes passos ao migrar para o WSUS 2.0 Service Pack 1 com uma configuração SQL remota:

1) Execute o pacote de configuração no front-end sem quaisquer comutadores e escolha a opção para actualizar

2) Execute o pacote de configuração no back-end sem quaisquer comutadores e escolha a opção para actualizar.

#### Copyright

As informações contidas neste documento representam a visão actual da Microsoft Corporation sobre os problemas discutidos na data de publicação. Como a Microsoft tem de responder a condições de mercado em constante mutação, não deverá ser interpretado como um compromisso da parte da Microsoft, e a Microsoft não pode garantir a precisão de qualquer informação apresentada a partir da data de publicação.

Este documento destina-se apenas a fins informativos. A MICROSOFT NÃO FORNECE QUALQUER GARANTIA, EXPRESSA, IMPLÍCITA OU LEGAL, ÀS INFORMAÇÕES DESTE DOCUMENTO.

É da responsabilidade do utilizador o cumprimento das leis de direitos de autor aplicáveis. Sem limitação dos direitos protegidos por copyright, nenhuma parte deste documento pode ser reproduzida, guardada ou introduzida em sistemas de dados, ou transmitida por qualquer forma ou meio (electrónico, mecânico, fotocópia, gravação ou outro), nem para quaisquer fins, sem o consentimento expresso, por escrito, da Microsoft Corporation.

A Microsoft pode ter patentes, pedidos de patentes, marcas comerciais, copyrights e outros direitos de propriedade intelectual sobre a matéria tratada neste documento. Salvo disposição expressa em qualquer contrato de licença escrito da Microsoft, o facto de este documento lhe ser fornecido não lhe concede quaisquer direitos ou licenças sobre essas patentes, marcas comerciais, direitos de autor ou outro tipo de propriedade intelectual.

Salvo indicação em contrário, os exemplos de empresas, organizações, produtos, nomes de domínios, endereços de correio electrónico, logótipos, pessoas, locais e eventos contidos neste documento são fictícios e não são intencionais nem devem inferir-se quaisquer associações a qualquer empresa, organização, produto, nome de domínio, endereço de correio electrónico, logótipo, pessoa, local ou evento real.

© 2005 Microsoft Corporation. Todos os direitos reservados.

Microsoft, SQL Server, Windows e Windows Server são marcas registadas ou marcas comerciais da Microsoft Corporation nos Estados Unidos e/ou noutros países.

Os nomes de empresas e produtos reais mencionados neste documento podem ser marcas comerciais dos respectivos proprietários.
