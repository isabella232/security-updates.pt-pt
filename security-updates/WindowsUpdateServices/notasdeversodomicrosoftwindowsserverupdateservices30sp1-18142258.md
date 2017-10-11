---
TOCTitle: 'Notas de Versão do Microsoft Windows Server Update Services 3.0 SP1'
Title: 'Notas de Versão do Microsoft Windows Server Update Services 3.0 SP1'
ms:assetid: 'a5aa93bf-842b-4ad4-ab0f-fe867843cb02'
ms:contentKeyID: 18142258
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc708525(v=WS.10)'
---

Notas de Versão do Microsoft Windows Server Update Services 3.0 SP1
===================================================================

Estas notas de versão descrevem problemas conhecidos que afectam o Microsoft® Windows® Server Update Services (WSUS) 3.0 Service Pack 1 e incluem recomendações e requisitos para a instalação da aplicação. Estas notas contêm as seguintes secções:

-   Requisitos de sistema para a instalação do servidor WSUS 3.0 SP1
-   Requisitos de configuração para a instalação do servidor WSUS 3.0 SP1
-   Requisitos de sistema para a instalação da consola remota WSUS 3.0 SP1
-   Requisitos do sistema para instalação de clientes
-   Requisitos de software para a instalação do servidor WSUS SP1
-   Requisitos mínimos de espaço em disco para a instalação do servidor WSUS 3.0 SP1
-   Requisitos de actualização do WSUS 3.0 SP1
-   Parâmetros de linha de comandos do programa de configuração
-   Problemas de configuração
-   Problemas de actualização
-   Problemas conhecidos
-   WSUS 3.0 SP1 no Windows Server® 2008
-   O WSUS 3.0 SP1 no Windows Small Business Server 2003

Requisitos de sistema para a instalação do servidor WSUS 3.0 SP1
----------------------------------------------------------------

#### O servidor WSUS 3.0 SP1 é suportado no Windows Server 2008 e no Windows Server 2003 Service Pack 1

O servidor WSUS 3.0 SP1 é suportado no Windows Server 2008 e no Windows Server 2003 Service Pack 1.

#### O Windows 2000 Server não é suportado para servidores WSUS 3.0 SP1

O Microsoft Windows® 2000 Server não é um sistema operativo suportado para servidores WSUS 3.0 SP1.

#### O WSUS 3.0 SP1 não é suportado em servidores a executar Serviços de Terminal

Embora o WSUS 3.0 SP1 ainda possa funcionar em servidores com Serviços de Terminal, tal procedimento não é suportado ou recomendado. Não será possível executar o WSUS 3.0 SP1 num servidor com Serviços de Terminal em configurações que utilizem implementações remotas do SQL Server. Uma vez que todas as acções personalizadas remotas (incluindo a instalação) num servidor de licença de Serviços de Terminal serão executadas como a conta do sistema e a conta do sistema do servidor pode não ter permissões no SQL Server remoto, a instalação pode falhar.

Requisitos de configuração para a instalação do servidor WSUS 3.0 SP1
---------------------------------------------------------------------

#### O IIS tem de estar instalado

O WSUS 3.0 SP1 requer Serviços de Informação Internet (IIS), que não está instalado por predifinição no Windows Server 2008 ou no Microsoft Windows Server 2003. Se tentar instalar o WSUS 3.0 SP1 sem o IIS, a Configuração do Windows Server Update Services apresentará uma mensagem de erro a indicar que o IIS não está instalado.

#### Se o IIS estiver a ser executado no modo de isolamento do IIS 5.0, a instalação falhará

Se tiver actualizado o servidor da versão Windows 2000 Server para a versão Windows Server 2003, o IIS pode estar a ser executado no modo de compatibilidade IIS 5.0. Também é possível activar o modo de isolamento do IIS 5.0 no Gestor de IIS. Este procedimento provoca a falha da instalação. Deve desactivar o modo de isolamento do IIS 5.0 antes de instalar o WSUS 3.0 SP1.

#### Se qualquer componente do IIS estiver instalado no modo de compatibilidade de 32 bits numa plataforma de 64 bits, a instalação do WSUS 3.0 SP1 pode falhar

Todos os componentes do IIS devem ser instalados no modo nativo em plataformas de 64 bits. A instalação pode falhar se qualquer componente do IIS estiver num modo de compatibilidade de 32 bits.

#### Os servidores proxy podem suportar apenas HTTP, ou HTTP e HTTPS

No WSUS 3.0 SP1, é possível que um servidor proxy suporte apenas HTTP. Deve ser configurado um segundo servidor proxy que execute HTTPS através da linha de comandos (**wsusutil configuresslproxy**) antes de configurar o servidor WSUS a partir do Assistente de Configuração ou da consola de Administração.

#### Se existirem dois ou mais Web sites em execução na porta 80, elimine-os todos excepto um antes de instalar o WSUS

Se tiver dois ou mais Web sites em execução na porta 80 (por exemplo, Windows® SharePoint® Services), elimine-os todos excepto um antes de instalar o WSUS. Caso contrário, os clientes poderão não conseguir efectuar a actualização automática.

#### Quando instalar o WSUS 3.0 SP1, pode ser necessário desactivar programas antivírus

Quando instalar o WSUS 3.0 SP1, pode ser necessário desactivar programas antivírus, antes de poder efectuar a instalação com êxito. Depois de desactivar o programa antivírus, reinicie o computador antes de iniciar a instalação do WSUS. Reiniciar o computador impede que os ficheiros sejam bloqueados quando o processo de instalação necessitar de aceder aos mesmos. Depois de concluir a instalação, certifique-se de que reactiva o programa antivírus. Visite o Web site do fornecedor do programa antivírus para saber os passos exactos de desactivação e reactivação do programa antivírus e a respectiva versão.

| ![](images/Cc708525.Caution(WS.10).gif)Atenção                                                                                                                                                                                                                   |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Esta solução pode tornar o computador ou a rede mais vulnerável a ataques de utilizadores maliciosos ou de software malicioso, tal como vírus. Esta solução não é recomendada, apenas é fornecida para que possa implementá-la conforme entender. Utilize esta solução por sua conta e risco. |

| ![](images/Cc708525.note(WS.10).gif)Nota                                                                                                                                                                                                                                          |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Os programas antivírus destinam-se a ajudar a proteger o computador contra vírus. Não transfira ou abra ficheiros a partir de origens que não considera fidedignas, não visite Web sites que não considera fidedignos, nem abra anexos de correio electrónico quando o programa antivírus estiver desactivado. |

#### O WSUS 3.0 SP1 requer que a opção de accionadores aninhados esteja activada no SQL Server

A opção de accionadores aninhados está activada por predefinição; no entanto, pode ser desactivada por um administrador do SQL Server.

Se planear utilizar uma base de dados SQL Server como arquivo de dados do Windows Server Update Services, o administrador do SQL Server deverá verificar se a opção de accionadores aninhados está activada antes de o administrador do WSUS 3.0 SP1 instalar o WSUS 3.0 SP1 e especificar a base de dados durante a configuração.

A Configuração do WSUS 3.0 SP1 activa a opção RECURSIVE\_TRIGGERS, que é uma opção específica de base de dados; no entanto, não activa a opção de accionadores aninhados, que é uma opção global de servidor.

Para ver se a opção de accionadores aninhados está activada, utilize:

**sp\_configure 'nested triggers'**

Para activar a opção de accionadores aninhados no SQL Server, execute o seguinte a partir de um ficheiro batch no computador com o SQL Server:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Se não tiver o SQL Server Management Studio no servidor, deve executar scripts de SQL a partir da linha de comandos. Pode obter o Utilitário de Consulta da Linha de Comandos do Microsoft SQL Server 2005 a partir do [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728). Para começar, execute **sqlcmd**.

Se pretender executar scripts de SQL no Base de dados interna do Windows, deve também transferir o SQL Server Native Client a partir da mesma página de transferência.

#### Requisitos e limitações de SQL remoto

O WSUS 3.0 SP1 oferece suporte para execução de software de base de dados num computador separado do computador que contém o resto da aplicação WSUS 3.0 SP1. Existem alguns requisitos para configurar uma instalação de SQL remoto:

-   Não é possível utilizar um servidor configurado como controlador de domínio do computador de back-end do par SQL remoto.
-   O computador que funcionará como servidor front-end de uma instalação remota de SQL não deve executar o Servidor de Terminais.
-   É necessário utilizar, pelo menos, o Microsoft SQL Server 2005 Pack 1 (disponível no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=66143) para software de base de dados em computadores de back-end para servidores com o Windows Server 2003, e o SQL Server 2005 Service Pack 2 para computadores de back end com o Windows Server® 2008.
-   Os computadores de front-end e de back-end devem estar integrados num domínio do Active Directory; caso contrário, se estiverem em domínios diferentes, é necessário estabelecer fidedignidade de domínio entre os domínios antes de executar a configuração do WSUS.
-   Se já tiver instalado o WSUS 2.0 numa configuração remota de SQL e pretender actualizar para o WSUS 3.0 SP1, deve desinstalar o WSUS 2.0 (utilizando **Adicionar ou Remover Programas** no Painel de Controlo) no computador de back-end, assegurando simultaneamente que a base de dados existente permanece intacta. Em seguida, deve instalar o SQL Server 2005 SP1 ou SP2 e actualizar a base de dados existente. Finalmente, deve instalar o WSUS 3.0 SP1 no computador de front-end.

Requisitos de sistema para a instalação da consola remota WSUS 3.0 SP1
----------------------------------------------------------------------

A consola remota WSUS 3.0 SP1 pode ser instalada nas seguintes plataformas:

-   Windows Server 2008
-   Windows Vista® ou posterior
-   Windows Server 2003 SP1 ou posterior
-   Windows XP SP2 ou posterior

Requisitos do sistema para instalação de clientes
-------------------------------------------------

A funcionalidade Actualizações Automáticas é o cliente de software do WSUS. Pode ser utilizada com o WSUS em qualquer um dos seguintes sistemas operativos:

-   Windows Vista ou posterior
-   Windows Server 2008 ou posterior
-   Microsoft Windows Server 2003, qualquer edição
-   Microsoft Windows XP Professional SP2 ou posterior
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 ou Windows 2000 Advanced Server com SP4

Requisitos de software para a instalação do servidor WSUS 3.0 SP1
-----------------------------------------------------------------

A tabela seguinte mostra o software necessário para as plataformas do Windows Server 2003 SP1. O software necessário para o Windows Server 2008 será abordado na secção que trata do WSUS 3.0 SP1 no Windows Server 2008.

Antes de executar o programa de configuração do WSUS 3.0 SP1, certifique-se de que o servidor WSUS 3.0 SP1 preenche esta lista de requisitos. Se algumas destas actualizações requerer que o computador seja reiniciado quando a instalação estiver concluída, deverá reiniciá-lo antes de instalar o WSUS 3.0 SP1.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Requisito</th>
<th style="border:1px solid black;" >Detalhes</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Serviços de Informação Internet da Microsoft (IIS)</td>
<td style="border:1px solid black;">Instale a partir do sistema operativo.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Version 2.0 Redistributable Package</td>
<td style="border:1px solid black;">Consulte Microsoft .NET Framework Version 2.0 Redistributable Package (x86) no <a href="http://go.microsoft.com/fwlink/?linkid=68935">Centro de Transferências da Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=68935). Para plataformas de 64 bits, consulte Microsoft .NET Framework Version 2.0 Redistributable Package (x64) no <a href="http://go.microsoft.com/fwlink/?linkid=70637">Centro de Transferências da Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70637)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Consola de Gestão da Microsoft 3.0 para Windows Server 2003</td>
<td style="border:1px solid black;">Trata-se de um pré-requisito para utilizar a interface de utilizador do WSUS 3.0 SP1. Consulte Consola de Gestão da Microsoft 3.0 para Windows Server 2003 (KB907265) no <a href="http://go.microsoft.com/fwlink/?linkid=70412">Centro de Transferências da Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70412). Para plataformas de 64 bits, consulte Consola de Gestão da Microsoft 3.0 para Windows Server 2003 x64 Edition (KB907265) no <a href="http://go.microsoft.com/fwlink/?linkid=70638">Centro de Transferências da Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70638).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Trata-se de um pré-requisito para utilizar a interface de utilizador do WSUS 3.0 SP1. Consulte Microsoft Report Viewer Redistributable 2005 no <a href="http://go.microsoft.com/fwlink/?linkid=70410">Centro de Transferências da Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (opcional)</td>
<td style="border:1px solid black;">O WSUS 3.0 SP1 instala o Base de dados interna do Windows se não houver uma versão compatível do SQL Server já instalada. Se planear utilizar uma base de dados SQL Server completa, deve utilizar (no mínimo) o SQL Server 2005 SP1 (disponível no <a href="http://go.microsoft.com/fwlink/?linkid=66143">Centro de Transferências da Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=66143) para o Windows Server 2003, ou o SQL Server 2005 SP2 (disponível no<a href="http://go.microsoft.com/fwlink/?linkid=84823">Centro de Transferências da Microsoft</a> em http://go.microsoft.com/fwlink/?LinkId=84823) no Windows Server 2008.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc708525.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                               |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Se o WSUS 2.0 já tiver sido instalado anteriormente e estiver a utilizar o SQL Server 2000, o SQL Server Desktop Engine 2000 ou qualquer base de dados do SQL Server anterior ao SQL Server 2005 SP1 (ou SQL Server 2005 SP2 no Windows Server 2008), o programa de instalação do WSUS 3.0 SP1 instalará oBase de dados interna do Windows® e migrará a base de dados para o mesmo. |
  
Requisitos mínimos de espaço em disco para a instalação do servidor WSUS 3.0 SP1  
--------------------------------------------------------------------------------
  
Os requisitos mínimos de espaço em disco para a instalação do Windows Server Update Services são os seguintes:
  
-   1 GB na partição do sistema  
-   2 GB para o volume no qual os ficheiros de base de dados serão armazenados  
-   20 GB para o volume onde o conteúdo será armazenado
  
| ![](images/Cc708525.Important(WS.10).gif)Importante                                         |  
|--------------------------------------------------------------------------------------------------------------------------|  
| Não é possível instalar o WSUS 3.0 SP1 em unidades comprimidas. Verifique se a unidade seleccionada não está comprimida. |
  
Requisitos de actualização do WSUS 3.0 SP1  
------------------------------------------
  
#### Verificar se a instalação do WSUS está a funcionar correctamente e fazer uma cópia de segurança da base de dados do WSUS antes da actualização
  
Se estiver a actualizar para o WSUS 3.0 SP1 a partir de uma versão anterior, certifique-se de que a instalação actual está a funcionar correctamente e efectue uma cópia de segurança da base de dados do WSUS antes da actualização.
  
1.  Verifique a existência de erros recentes nos registos de eventos, problemas de sincronização entre servidores a jusante e servidores a montante ou problemas com clientes que não estejam a comunicar. Certifique-se de que esses problemas foram resolvidos antes de continuar.  
2.  Execute o comando DBCC CHECKDB para garantir que a base de dados do WSUS está indexada correctamente. Para obter mais informações sobre o comando DBCC CHECKDB, consulte [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948).  
3.  Faça a cópia de segurança da base de dados do WSUS.
  
#### Se tiver modificado manualmente a porta utilizada pelo WSUS, desinstale-a antes da actualização
  
Quando modificar a porta do WSUS, utilize sempre o utilitário wsusutil em vez de tentar modificar a porta manualmente. Se tiver modificado manualmente a porta e tiver actualizado anteriormente do Software Update Services 1.0 para o WSUS 2.0:
  
1.  Se ainda não instalou o WSUS 3.0, desinstale o WSUS 2.0, mantendo a base de dados e o conteúdo. (Se já tiver instalado o WSUS 3.0, desinstale-o, mantendo a base de dados e o conteúdo)  
2.  Inicie o Web site Predefinido, reactivando temporariamente o SUS 1.0, mas mantendo-o acessível para o desinstalador.  
3.  Desinstale o SUS 1.0.  
4.  Instale o WSUS 3.0.
  
#### O Software Update Services 1.0 deve ser desinstalado
  
Não é possível instalar o WSUS 3.0 SP1 se o Software Update Services 1.0 estiver instalado no mesmo computador. Deve desinstalar o Software Update Services 1.0 antes de instalar o WSUS 3.0 SP1.
  
#### Não é possível actualizar do WSUS 2.0 para o WSUS 3.0 SP1 num sistema operativo de 64 bits
  
O WSUS 2.0 não é suportado em sistemas operativos de 64 bits. Não é possível actualizar do WSUS 2.0 para o WSUS 3.0 SP1 em sistemas operativos de 64 bits.
  
Parâmetros de linha de comandos do programa de configuração  
-----------------------------------------------------------
  
É possível efectuar instalações automáticas do WSUS 3.0 SP1, utilizando os parâmetros da linha de comandos do WSUS. Esta tabela mostra os parâmetros de linha de comandos do programa de configuração do WSUS 3.0 SP1.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Opção</th>
<th style="border:1px solid black;" >Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Executar instalação silenciosa.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Desinstalar o produto. Também desinstala a instância do Base de dados interna do Windows se este estiver instalado.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Apenas verificação de pré-requisito. Não instala o produto, mas inspecciona o sistema e comunica eventuais pré-requisitos em falta.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Mostra os parâmetros de linha de comandos e as respectivas definições.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Actualização a partir da versão anterior do WSUS. (Não tente actualizar a partir do SUS 1.0.) O único parâmetro válido com esta opção é /q (instalação silenciosa). A única propriedade válida com esta opção é DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
Esta tabela mostra as propriedades de linha de comandos para o WSUS 3.0 SP1.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Propriedade</th>
<th style="border:1px solid black;" >Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0 = conteúdo alojado localmente, 1 = alojar no Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Caminho para o directório de conteúdo. A predefinição é <em>UnidadeInstalaçãoWSUS</em><strong>\WSUS\WSUSContent</strong>, em que <em>UnidadeInstalaçãoWSUS</em> é a unidade local com mais espaço de disco disponível.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Caminho para o directório de dados Base de dados interna do Windows.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Este nome deve ser apresentado no formato <em>NomeServidor</em>\<em>NomeInstânciaSQL</em>. Se a instância de base de dados estiver no computador local, utilize a variável de ambiente %COMPUTERNAME%. Se não estiver presente uma instância existente, a predefinição é %COMPUTERNAME%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0 = porta 8530, 1 = porta 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Caminho e nome de ficheiro do ficheiro de registo</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0 = instalar o servidor WSUS, 1 = instalar apenas a consola</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0 = não instalar funcionalidades de inventário, 1 = instalar funcionalidades de inventário</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0 = reter base de dados, 1 = remover base de dados</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0 = reter ficheiros de conteúdo, 1 = remover ficheiros de conteúdo</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0 = reter ficheiros de registo, 1 = remover ficheiros de registo (utilizado com o parâmetro /u de instalação).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0 = utilizar base de dados actual, 1 = criar base de dados</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Identificador de janela para devolver mensagens de progresso MSI</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1 = participar no Programa de Melhoramento do Microsoft Update, 0 = não participar no Programa de Melhoramento do Microsoft Update</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1 = não escrever a localização de conteúdo na base de dados, 0 = escrever a localização de conteúdo na base de dados (para NLB)</td>
</tr>
</tbody>
</table>
  
#### Utilização de Exemplo
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](images/Cc708525.Important(WS.10).gif)Importante                                                                                                                                        |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Se instalar o WSUS 3.0 SP1 no modo silencioso (/q) e o computador não tiver todos os pré-requisitos instalados, a instalação irá gerar um ficheiro com o nome WSUSPreReqCheck.xml e irá guardá-lo no directório %TEMP%. |
  
Problemas de configuração  
-------------------------
  
#### O IIS será reiniciado durante a Configuração do WSUS 3.0 SP1
  
O Programa de Configuração do WSUS 3.0 SP1 irá reiniciar o IIS sem notificação, o que poderá afectar Web sites existentes na organização. Se o IIS não estiver em execução, será iniciado pelo programa de configuração do WSUS 3.0 SP1.
  
#### Se estiverem abertas ligações para uma base de dados existente do WSUS, a instalação pode falhar
  
Se estiver a actualizar para o WSUS 3.0 SP1 a partir de uma instalação existente e ainda estiverem abertas as ligações à base de dados WSUS existente (por exemplo, se o SQL Server Management Studio estiver aberto), a instalação pode falhar. Feche todas as ligações e reinstale o WSUS 3.0 SP1.
  
#### A configuração do WSUS mostra o directório errado para os ficheiros de base de dados
  
Na configuração do WSUS, o ecrã **Pronto para Instalar** indica incorrectamente que o directório principal é a localização da base de dados. Por exemplo, a localização predefinida é %systemdrive%\\WSUS\\UpdateServicesDbFiles, mas esta localização aparece incorrectamente como %systemdrive%\\WSUS.
  
#### Se o WSUS for instalado num computador que tem pacotes de idiomas do Multilingual User Interface com um idioma predefinido diferente do inglês, a Ajuda será apresentada no idioma predefinido e não em inglês
  
Se tiver um computador que tem pacotes de idiomas do Multilingual User Interface com um idioma predefinido diferente do inglês, ainda é possível instalar o WSUS se a região actual do utilizador for inglês. A IU será apresentada em inglês, mas deve utilizar uma solução para apresentar a Ajuda em inglês. Copie o ficheiro .chm da Ajuda em inglês (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) para o directório principal de documentação (*WSUSInstallDir*\\documentation\\WSUS30Help.chm). Desta forma, a Ajuda deve ser apresentada correctamente em todos os idiomas.
  
Problemas de actualização  
-------------------------
  
#### Recuperar de uma actualização com falha
  
Se estiver a actualizar de uma versão anterior do WSUS (WSUS 3.0, WSUS 2.0 SP1 ou WSUS 2.0) para o WSUS 3.0 SP1 e a actualização falhar por qualquer motivo:
  
1.  Reinstale a versão anterior do WSUS.  
2.  Restaure a base de dados a partir da cópia de segurança efectuada antes de tentar actualizar. (Na maior parte dos casos, o WSUS também cria automaticamente uma cópia de segurança. Consulte o ficheiro WSUSSetup.log para obter a localização).  
3.  Analise os ficheiros de registo para determinar a causa da falha e corrija o problema.  
4.  Tente actualizar o WSUS novamente.
  
#### Não é possível actualizar do WSUS 2.0 para o WSUS 3.0 SP1, se existir uma base de dados WSUS 3.0 SP1 de uma instalação anterior
  
Se já tiver instalado anteriormente o WSUS 3.0 SP1 e, em seguida, tiver reinstalado o WSUS 2.0, tem de eliminar a base de dados do WSUS 3.0 SP1 do computador, antes de tentar reinstalar o WSUS 3.0 SP1.
  
#### A alteração do nome do computador antes da actualização para o WSUS 3.0 SP1 pode fazer com que a actualização falhe
  
Se alterar o nome do computador depois de instalar o WSUS 2.0 e antes de actualizar para o WSUS 3.0 SP1, a actualização pode falhar.
  
Utilize o seguinte script para remover e voltar a adicionar os grupos ASPNET e Administradores WSUS. Em seguida, execute novamente a actualização.
  
Será necessário substituir*&lt;DBLocation&gt;* pela pasta em que está instalada a base de dados e *&lt;ContentDirectory&gt;* pela pasta de armazenamento local.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### A Configuração substituirá uma cópia de segurança da base de dados anterior
  
A configuração do WSUS 3.0 SP1 adicionará a base de dados ao directório predefinido, que é *unidade*\\WSUS (em que *unidade* é a unidade NTFS local que possui maior espaço de disco disponível). Se houver uma cópia de segurança da base de dados neste directório, poderá ser substituída. Os administradores devem guardar uma cópia de segurança da base de dados da versão actual numa localização diferente antes da actualização para o WSUS 3.0 SP1.
  
#### Se tiver migrado de MSDE para SQL Server 2000 ou SQL Server 2005 em WSUS 3.0, é necessário alterar um valor do registo
  
Se tiver uma instalação do WSUS 2.0 e tiver migrado para SQL Server 2000 ou SQL Server 2005, deve alterar o valor **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** de 1 para 0. Se não o fizer antes de actualizar para o WSUS 3.0 SPQ, a actualização falhará.
  
#### Se a configuração do WSUS 2.0 for iniciada e cancelada, eliminará a chave do registo WSUS
  
Se iniciar a configuração do WSUS 2.0 e, em seguida, a cancelar, a chave do registo WSUS será eliminada. Isso pode originar problemas se já tiver o WSUS 3.0 SP1 instalado. O mesmo problema ocorrerá se iniciar a desinstalação do WSUS 2.0, cancelar a operação e, em seguida, tentar efectuar a actualização do WSUS 2.0 para o WSUS 3.0 SP1.
  
#### Se desinstalar o WSUS 3.0 e se esquecer dos ficheiros de registo, estes poderão não ter as permissões correctas após a reinstalação
  
Quando desinstalar o WSUS 3.0 SP1, tem a opção de manter os ficheiros de registo da instalação. Ao reinstalar o WSUS 3.0, os ficheiros de registo antigos perdem as respectivas permissões (normalmente, apenas para Administradores WSUS). Deverá restaurar as permissões para estes ficheiros de registo.
  
#### Se os clientes WSUS 2.0 tiverem actualizações com o estado “Não Aplicável”, as actualizações aparecerão como “Desconhecido” durante um curto período de tempo após a actualização para o WSUS 3.0 SP1
  
Se um servidor WSUS 2.0 tiver clientes com actualizações **Não Aplicável** estas actualizações aparecerão com o estado**Desconhecido** durante um curto período de tempo após a actualização do servidor para o WSUS 3.0 SP1. O estado da actualização regressará a **Não Aplicável** depois da próxima vez que o cliente fizer uma procura.
  
Problemas Conhecidos  
--------------------
  
#### Resolução de múltiplos erros de transferência ou de repetidas falhas de sincronização de cliente
  
Se os clientes do WSUS 3.0 SP1 relatarem múltiplos erros de transferência ou se os clientes não conseguirem sincronizar com o servidor WSUS 3.0 SP1 durante um longo período de tempo, pode ter uma cache de transferência de cliente danificada. Para recuperar deste estado, pode tentar eliminar a cache de transferência do cliente a partir do sistema de ficheiros.
  
Para eliminar a cache de transferência do cliente:
  
1.  Elimine todos os ficheiros e subdirectórios nesta localização no computador cliente: **%windir%\\SoftwareDistribution\\Download**  
2.  Tente instalar a actualização sincronizando o computador cliente com o WSUS 3.0 SP1 novamente. Esta tentativa de instalação deverá falhar, com a seguinte mensagem de erro: **WU\_E\_DM\_NOTDOWNLOADED, "A actualização não foi transferida."**  
3.  Depois desta falha, o computador cliente irá automaticamente reiniciar a transferência e a instalação poderá prosseguir.
  
#### Se ocorrer uma falha na sincronização, tente executá-la novamente
  
Se a sincronização falhar, a primeira medida para resolução de problemas deve ser tentar sincronizar o servidor novamente. Se as sincronizações subsequentes falharem, utilize as informações de resolução de problemas do [Guia de Funcionamento do Windows Server Update Services 3.0](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072).
  
#### A alteração da configuração do WSUS 3.0 SP1 directamente na base de dados não é suportada
  
O Windows Server Update Services armazena os respectivos dados de configuração numa base de dados do SQL Server. No entanto, a alteração dos dados de configuração acedendo directamente à base de dados não é suportada. Não tente modificar a configuração do WSUS 3.0 SP1 acedendo directamente à base de dados. Deve alterar a configuração do WSUS 3.0 SP1 utilizando a consola WSUS 3.0 SP1 ou iniciando as APIs do WSUS 3.0 SP1.
  
#### As falhas de transferência não são relatadas rapidamente se as quotas de disco estiverem activadas
  
Se as quotas de disco estiverem activadas e a quota for atingida, as falhas de transferência de actualização no WSUS podem não ser relatadas de forma atempada. Para evitar esta situação, desactive as quotas de disco ou aumente a quota.
  
#### Se o WSUS 3.0 SP1 for implementado utilizando SSL, os computadores cliente podem falhar com um código de erro de "0x8024400a"
  
Os computadores cliente podem, por vezes, apresentar uma falha com um código de erro "0x8024400a" ao comunicarem com um servidor WSUS 3.0 SP1 utilizando SSL. Para obter uma actualização que resolva este problema, consulte o artigo[KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593).
  
#### A conta de domínio dos Administradores WSUS não será eliminada se o WSUS for desinstalado
  
O grupo Administradores WSUS é criado como uma conta de domínio (não uma conta local) em controladores de domínio, por isso todas as instalações que utilizam esta conta de domínio seriam desactivadas se a conta fosse eliminada no decurso da desinstalação do WSUS. Por conseguinte, a desinstalação do WSUS não eliminará a conta de domínio Administradores WSUS.
  
#### Se um servidor a jusante for convertido num servidor a montante, é necessário reimportar as actualizações de site de catálogo
  
Se tornar um servidor a jusante num servidor a montante, também tem de reimportar todas as actualizações do site de catálogo. Caso contrário, o site não conseguirá sincronizar as novas revisões de actualização de site do catálogo para este servidor.
  
#### Se estiver a utilizar o IIS com SSL, o acesso não encriptado continua a ser possível, a menos que esteja seleccionada a opção "Requerer Canal Seguro"
  
Se configurar o IIS para utilizar SSL instalando um certificado, ainda é possível aceder ao site através de HTTP não encriptado, a menos que esteja seleccionada a opção **Requerer Canal Seguro**. Para obter mais informações, consulte a documentação do [IIS](http://go.microsoft.com/fwlink/?linkid=98084) (http://go.microsoft.com/fwlink/?LinkId=98084).
  
#### A importação do site do catálogo pode falhar sem permissões de leitura/escrita para a pasta %windir%\\TEMP
  
Ao efectuar uma importação do site do catálogo, se a conta Serviço de Rede não tiver permissão de leitura/escrita para a pasta %windir%\\TEMP, a importação pode falhar apresentando uma mensagem de erro como a seguinte: O servidor não conseguiu processar o pedido. ---&gt; Não foi possível localizar o ficheiro “C:\\WINDOWS\\TEMP\\*NomeFicheirotemporário*.dll".
  
#### O desempenho pode ser lento ao sincronizar entre o WSUS 3.0 SP1 e um servidor de réplica a jusante com o WSUS 2.0
  
Se instalar o WSUS 3.0 SP1 num servidor a montante e tentar sincronizar com um servidor de réplica a jusante com o WSUS 2.0, pode ter problemas de desempenho. Para resolver este problema, consulte o artigo [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669).
  
#### Se o servidor de correio estiver indisponível ou inacessível, a notificação por correio electrónico falha sem aviso prévio
  
Se o servidor de correio electrónico da rede estiver offline, o WSUS 3.0 SP1 não enviará notificações por correio electrónico, nem apresentará um aviso para o efeito. No entanto, escreverá o evento 10052 (HealthCoreEmailNotificationRed) no registo de eventos.
  
#### As definições alteradas num servidor a montante não serão imediatamente aplicadas no servidor a jusante
  
Quando a configuração do servidor a montante for alterada, pode demorar algum tempo antes de estas alterações de configuração entrarem em vigor. Por exemplo, se alterar uma definição no servidor a montante, tal como a selecção de um novo idioma, e accionar imediatamente uma sincronização no servidor a jusante, a alteração não será apresentada. Em vez disso, será aplicada ao servidor a jusante na próxima sincronização agendada. O tempo de espera aumenta consoante o número de actualizações existentes no servidor a montante.
  
#### Desinstalar o WSUS 3.0 SP1 não desinstala a instância de base de dados
  
Se o WSUS 3.0 SP1 for desinstalado, a instância de base de dados não será desinstalada. A instância pode ser partilhada por mais de uma aplicação, causando a falha de outras aplicações se for removida.
  
Se for necessário desinstalar o Base de dados interna do Windows, os seguintes comandos desinstalam a aplicação:
  
(em plataformas de 32 bits)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(em plataformas de 64 bits)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Se pretende desinstalar o Base de dados interna do Windows o Service Pack 2 do Windows Server 2008, poderá fazê-lo através do Server Manager.
  
No entanto, a remoção da aplicação pode não remover os ficheiros .mdf e .ldf predefinidos, o que irá causar a falha da subsequente instalação do WSUS 3.0 SP1. Estes ficheiros podem ser eliminados no directório %windir%\\SYSMSI\\SSEE.
  
#### Se um servidor a jusante alterar o servidor a montante, as actualizações de estado “Desconhecido” são relatadas como sendo “Não Aplicável”
  
Se um servidor a jusante começar a sincronizar a partir de um servidor a montante diferente, as actualizações que têm um estado **Desconhecido** serão relatadas no novo servidor a montante como **Não Aplicável**. Este estado é temporário e será corrigido na próxima vez que o servidor a montante relatar o seu estado, depois de os respectivos clientes terem efectuado a sincronização com o mesmo.
  
#### Se o tempo limite do Assistente de Limpeza do Servidor for excedido ao ser executado em múltiplos servidores a partir de uma consola remota, será perdida a ligação a todos os servidores
  
É possível executar o Assistente de Limpeza do Servidor em múltiplos servidores a partir de uma consola remota. No entanto, se o tempo limite do processo de limpeza se esgotar num dos servidores, a consola perderá a sua ligação a todos os servidores. Não serão perdidos dados, mas o administrador terá de repor a ligação remota a cada um dos servidores.
  
#### Iniciar e parar a ligação numa sucessão rápida gera a mensagem de erro "Não ocorreu nenhuma falha de sincronização" no Assistente de Configuração
  
Ao configurar o WSUS, é necessário estabelecer ligação ao servidor a montante (o servidor a montante da intranet ou do Microsoft Update) para transferir informações básicas sobre o servidor. Se clicar em **Iniciar Ligação** e clicar de imediato em **Parar Ligação**, receberá a mensagem de erro incorrecta "Não ocorreu nenhuma falha na sincronização".
  
O WSUS 3.0 SP1 no Windows Server 2008  
-------------------------------------
  
#### Versões Suportadas
  
O WSUS 3.0 SP1 suporta o Windows Server 2008 nas versões de 32 e 64 bits.
  
#### Pré-requisitos
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Requisito</th>
<th style="border:1px solid black;" >Detalhes</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Serviços de Informação Internet da Microsoft (IIS)</td>
<td style="border:1px solid black;">Instale a partir do sistema operativo. Certifique-se de que os seguintes componentes estão activados:
<ul>
<li>Autenticação do Windows<br />
<br />
</li>
<li>Conteúdo Estático<br />
<br />
</li>
<li>ASP.NET<br />
<br />
</li>
<li>Compatibilidade de Gestão do 6.0<br />
<br />
</li>
<li>Compatibilidade da Metabase do IIS 6.0<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Version 2.0 Redistributable Package (x86)</td>
<td style="border:1px solid black;">Desnecessário no Windows Server 2008; já instalado como parte do sistema operativo.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Consola de gestão da Microsoft 3.0</td>
<td style="border:1px solid black;">Desnecessário no Windows Server 2008; já instalado como parte do sistema operativo.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Trata-se de um pré-requisito para utilizar a interface de utilizador do WSUS. Consulte Microsoft Report Viewer Redistributable 2005 no <a href="http://go.microsoft.com/fwlink/?linkid=70410">Centro de Transferências da Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
</tbody>
</table>
  
#### Utilizar o Assistente de Configuração de Segurança
  
No Windows Server 2008, quando executar o Assistente de Configuração de Segurança (SCW), pode seleccionar a função do WSUS e activar as respectivas dependências. Para executar o SCW, clique em **Iniciar**, aponte para **Ferramentas Administrativas**, e, em seguida, clique em **Assistente de Configuração de Segurança**.
  
Os problemas conhecidos seguintes existem com a utilização conjunta do SCW e da função do WSUS:
  
-   **O serviço do Base de Dados Interna do Windows é activada, embora possa não ser utilizada pelo WSUS.** O WSUS é configurado para utilizar uma base de dados - o Base de Dados Interna do Windows ou a base de daos do SQL. Se o WSUS for instalado com o SQL Server e seleccionar a função do WSUS no SCW, o Base de Dados Interna do Windows é activado, se estiver instalado no computador, mas não é utilizado pelo WSUS. Deve desactivar o serviço do Base de Dados Interna do Windows se estiver a utilizar a base de dados do SQL Server em vez do Base de Dados Interna do Windows.  
-   **As regras de firewall para o WSUS num Web site personalizado não estão seleccionadas por predefinição.** Se instalar o WSUS num Web site personalizado (porta 8530 ou 8531), as regras da firewall não estão automaticamente seleccionadas, mesmo que seleccione a função do WSUS no SCW. Deve activar as regras de firewall adequadas para o WUSUS baseadas no facto de o protocolo Secure Sockets Layer (SSL) estar configurado para o servidor WSUS.
  
O WSUS 3.0 SP1 no Windows Small Business Server 2003  
----------------------------------------------------
  
#### Se a raiz virtual do IIS estiver restringida a determinados endereços IP ou nomes de domínio, o servidor WSUS 3.0 SP1 não conseguirá actualizar-se automaticamente
  
Algumas instalações do Windows Small Business Server podem ter o Web site predefinido do IIS configurado para **restrições de endereço IP e nome domínio**. Neste caso, o Cliente Windows Update no servidor poderá não conseguir efectuar a actualização automaticamente
  
#### Instalar o WSUS 3.0 SP1 no Small Business Server — Problemas de Integração
  
-   Se o Windows Small Business Server 2003 utilizar um servidor proxy ISA para aceder à Internet, terá de introduzir o seguinte na interface de utilizador **Definições** : **definições do servidor proxy, nome do servidor proxy e porta**.  
-   ISe o ISA estiver a utilizar a Autenticação do Windows, as credenciais do servidor proxy deverão ser escritas sob a forma *DOMÍNIO*\\*utilizador* e o utilizador deve pertencer ao grupo Utilizadores Internet.
  
#### Se tiver adicionado uma sub-rede à rede sem utilizar os assistentes do Windows SBS, deve efectuar o procedimento seguinte
  
O processo de configuração do servidor WSUS instala duas raízes virtuais do IIS no servidor: SelfUpdate e ClientWebService. O Programa de Configuração também coloca alguns ficheiros no directório raiz do Web site predefinido (na porta 80), o que permite aos computadores cliente actualizarem-se automaticamente através do Web site predefinido. Por predefinição, o Web site predefinido está configurado para recusar acesso a qualquer endereço IP que não o localhost ou sub-redes específicas ligadas ao servidor. Como resultado, os computadores cliente que não se encontrem no localhost ou nessas sub-redes específicas não podem actualizar-se automaticamente. Se tiver adicionado uma sub-rede à rede sem utilizar os assistentes do Microsoft Windows Small Business Server 2003 (Windows SBS), deve efectuar o procedimento seguinte:
  
1.  Em Gestão do Servidor, expanda **Gestão Avançada**, expanda **Serviços de Informação Internet**, expanda **Web Sites**, expanda **Web Site Predefinido**, clique com o botão direito do rato no directório virtual **Selfupdate** e, em seguida, clique em **Propriedades**.  
2.  Clique em **Segurança de Directórios**.  
3.  Em **restrições de endereço IP e nome domínio**, clique em **Editar**, e, em seguida, clique em **Acesso Concedido**.  
4.  Clique em **OK**, clique com o botão direito do rato no directório virtual **ClientWebService** e, em seguida, clique em **Propriedades**.  
5.  Clique em **Segurança de Directórios**.  
6.  Em **restrições de endereço IP e nome domínio**, clique em **Editar**, e, em seguida, clique em **Acesso Concedido**.
  
Copyright  
---------
  
As informações contidas neste documento, incluindo URLs e outras referências a Web sites, estão sujeitas a alterações sem aviso prévio. Salvo indicação expressa em contrário, os nomes de empresas, organizações, produtos, nomes de domínio, endereços de correio electrónico, logótipos, pessoas, locais e eventos mencionados neste documento são fictícios. Não se pretende nem deve ser inferida a representação de qualquer empresa, organização, produto, nome de domínio, endereço de correio electrónico, logótipo, pessoa, local ou evento real. É da responsabilidade do utilizador agir em conformidade com todas as leis de direito de autor aplicáveis. Sem limitação para os direitos de autor, nenhuma parte deste documento pode ser reproduzida, armazenada ou introduzida num sistema de recuperação, ou transmitida sob qualquer forma ou por qualquer meio (electrónico, mecânico, fotocópia, gravação ou outro), para qualquer fim, sem a permissão expressa, por escrito, da Microsoft Corporation.
  
Neste documento, podem ser feitas referências a patentes ou a pedidos de patentes pendentes, marcas comerciais, direitos de autor ou outros direitos de propriedade intelectual da Microsoft. Salvo disposição expressa em qualquer contrato de licença escrito da Microsoft, o facto de este documento lhe ser fornecido não lhe concede quaisquer direitos sobre essas patentes, marcas comerciais, direitos de autor ou outro tipo de propriedade intelectual.
  
© 2007 Microsoft Corporation. Todos os direitos reservados.
  
Microsoft, SQL Server, Windows e Windows Server são marcas registadas ou comerciais da Microsoft Corporation nos Estados Unidos e/ou noutros países.
  
Todas as restantes marcas comerciais são propriedade dos respectivos proprietários.
