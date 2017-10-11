---
TOCTitle: Notas de lançamento dos Serviços de Gestão de Direitos do Windows com o Service Pack 2
Title: Notas de lançamento dos Serviços de Gestão de Direitos do Windows com o Service Pack 2
ms:assetid: '78067886-681f-49a6-b43d-bfd08a369b69'
ms:contentKeyID: 18124058
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747637(v=WS.10)'
---

Notas de lançamento dos Serviços de Gestão de Direitos do Windows com o Service Pack 2
======================================================================================

*Data de lançamento: Dezembro de 2006*

Antes de começar
----------------

Consulte as seguintes informações antes de instalar os Serviços de Gestão de Direitos (RMS, Rights Management Services) do Microsoft® Windows® com o Service Pack 2 (SP2). As informações nestas notas de lançamento aplicam-se ao servidor RMS com SP2 e não ao cliente RMS. Para mais informações sobre clientes RMS, consulte as informações sobre Serviços de Gestão de Direitos ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)).

#### Requisitos do sistema

Os requisitos de hardware para utilizar o RMS com SP2 são apresentados na tabela seguinte.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Requisito</th>
<th>Recomendação</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Computador com um processador Pentium III (800 MHz ou superior)</td>
<td style="border:1px solid black;">Computador com dois processadores Pentium 4 (1500 MHz ou superior)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">256 MB de RAM</td>
<td style="border:1px solid black;">512 MB de RAM</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">20 GB de espaço livre no disco rígido</td>
<td style="border:1px solid black;">40 GB de espaço livre no disco rígido</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Nota                                                                               |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------|  
| O servidor RMS com SP2 foi concebido para um computador de 32 bits. Se for instalado num computador de 64 bits, será executado no modo de emulação. |
  
Os requisitos de software para os servidores a utilizar o RMS com SP2 são apresentados na tabela seguinte.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Componente</th>
<th>Requisito</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Sistema operativo</td>
<td style="border:1px solid black;">Microsoft Windows Server® 2003, excepto Web Edition, para o RMS com SP2.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Serviços de Gestão de Direitos com SP2</td>
<td style="border:1px solid black;">Deve instalar o RMS com o Service Pack 1 (SP1) antes de actualizar para o RMS com SP2. O cliente RMS com SP2 não possui este requisito.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Sistema de ficheiros</td>
<td style="border:1px solid black;">É recomendado o sistema de ficheiros NTFS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pré-requisitos de componentes</td>
<td style="border:1px solid black;"><ul>
<li>Colocação de Mensagens em Fila (também conhecida por MSMQ) com a integração do serviço de directório do Active Directory® activada.<br />
<br />
</li>
<li>Serviços de informação Internet (IIS) com o ASP.NET activado.<br />
<br />
</li>
<li>Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

| ![](images/Cc747637.note(WS.10).gif)Nota                                                                                                                                 |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se configurar o RMS com SP2 para permitir uma administração remota, o computador que efectua a ligação ao serviço de administração do RMS com SP2 deve utilizar o Internet Explorer 6.0 ou posterior. |

Os requisitos de infra-estrutura para os servidores a utilizar o RMS com SP2 são apresentados na tabela seguinte.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Componente</th>
<th>Requisitos</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Serviços de directório</td>
<td style="border:1px solid black;">Active Directory em controladores de domínios que utilizam o Windows Server 2000 com o Service Pack 3 (SP3) ou superior, no mesmo domínio em que o RMS está instalado. Todos os utilizadores e grupos que utilizam o RMS para adquirir licenças e publicar conteúdos deverão ter um endereço de correio electrónico configurado no Active Directory.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Servidor da base de dados</td>
<td style="border:1px solid black;">O RMS com SP2 necessita de uma base de dados e de procedimentos de armazenamento para efectuar as operações. Pode utilizar o Microsoft SQL Server™ 2000 com o SP3a ou posterior ou o Microsoft SQL Server 2005. Para realizar testes ou outras implementações em computadores individuais, é possível utilizar o Microsoft SQL Server Desktop Engine (MSDE 2000) Release A ou o Microsoft SQL Server 2005 Express Edition.</td>
</tr>
</tbody>
</table>
  
O RMS foi concebido e testado para servidores de bases de dados que utilizam o Microsoft SQL Server 2000 e o Microsoft SQL Server 2005. O RMS pode ser executado noutros servidores de bases de dados que obedeçam aos seguintes critérios:
  
-   Suporte de interfaces ADO.NET fornecidas pelo Microsoft .NET Framework 1.1.  
-   Compatibilidade com Transact-SQL, a linguagem de consulta estruturada que o Microsoft SQL Server utiliza, uma vez que os scripts de inicialização do RMS e os procedimentos armazenados do RMS utilizam Transact-SQL.  
-   Suporte para todas as extensões específicas do Microsoft SQL Server.  
-   Resposta a chamadas de métodos do espaço de nomes System.Data.SqlClient do .NET Framework.  
-   Fornecimento da respectiva funcionalidade do espaço de nomes System.Data.SqlClient.  
-   Utilização do Modo de Autenticação do Windows.
  
Para descobrir se o servidor da base de dados suporta os critérios acima descritos, contacte o respectivo fornecedor da base de dados.
  
A tabela seguinte apresenta as permissões e os direitos de utilizador necessários para efectuar diferentes actividades no RMS.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Actividade</th>
<th>Requisitos de conta</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Instalar o RMS</td>
<td style="border:1px solid black;">Utilizador do domínio com credenciais de administrador do computador local</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aprovisionar um cluster de raiz do RMS</td>
<td style="border:1px solid black;">Utilizador de domínio com credenciais de administrador do computador local e capacidade de escrita e pesquisa no Active Directory</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Aprovisionamento de um cluster apenas de licenciamento do RMS</td>
<td style="border:1px solid black;">Utilizador de domínio com credenciais de administrador do computador local e capacidade de pesquisa no Active Directory</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aprovisionamento utilizando uma nova base de dados de configuração</td>
<td style="border:1px solid black;">Utilizador de domínio com credenciais de administrador do computador local e capacidade de leitura, escrita e criação no computador com o SQL Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Aprovisionamento utilizando uma base de dados de configuração existente</td>
<td style="border:1px solid black;">Utilizador de domínio com credenciais de administrador do computador local e capacidade de leitura e escrita no computador com o servidor da base de dados</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Administração do RMS</td>
<td style="border:1px solid black;">Utilizador do domínio com credenciais de administrador do computador local</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Nota                                                                                                                                                                                                                  |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Para mais informações sobre a configuração do Windows Server, Active Directory, Colocação de Mensagens em Fila, IIS e sistemas de ficheiros, consulte o Windows Server 2003 TechCenter ([http://go.microsoft.com/fwlink/?LinkId=78135](http://go.microsoft.com/fwlink/?linkid=78135)). |
  
Se estiver a utilizar o RMS numa implementação de cluster, certifique-se de que tratou dos itens listados na tabela seguinte.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Condição</th>
<th>Recomendação</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Grande número de ambientes de trabalho que utilizarão o RMS</td>
<td style="border:1px solid black;">Utilize o Systems Management Server (SMS) ou a Política de Grupo para instalar o cliente RMS com SP2.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Grande número de pedidos de clientes</td>
<td style="border:1px solid black;">Utilize um servidor de balanceamento de carga, o serviço de Balanceamento de Carga em Rede no sistema operativo Windows Server, ou o balanceamento de carga do hardware para distribuir os pedidos pelo cluster.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Duas placas de rede com endereçamento IP virtual para pedidos de serviço da extranet e da intranet</td>
<td style="border:1px solid black;">Certifique-se de que qualquer registo de Sistema de Nomes de Domínio (DNS) que exponha o endereço de IP virtual à extranet também expõe o endereço à intranet.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.Important(WS.10).gif)Importante                                                                                                                                                                                                                                                                                                                                                                                                                |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Se o registo DNS não for efectuado para a intranet, os pedidos de licenciamento de clientes internos falharão. Se não for possível modificar as definições DNS, a tabela de anfitriões de cada servidor pode ser modificada para mapear o URL do cluster para o endereço IP virtual do cluster. É necessário efectuar o registo DNS antes de aprovisionar o RMS. Se o serviço já estiver aprovisionado, deverá remover o RMS do servidor e, em seguida, repetir o processo de aprovisionamento. |
  
#### Clientes suportados por esta versão
  
O cliente do RMS sem qualquer Service Pack, cliente do RMS com SP1 ou cliente do RMS com SP2 pode ser instalado em qualquer computador com o Microsoft Windows 2000, Windows XP e Windows Server 2003. Os sistemas operativos Windows de versões anteriores não são suportados por esta versão.
  
| ![](images/Cc747637.Caution(WS.10).gif)Atenção                                                                                                  |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Se estiver a utilizar o cliente do RMS sem qualquer Service Pack, o cliente não poderá utilizar a publicação online, por oposição a um servidor do RMS com SP1 ou posterior. |
  
Alterações às funcionalidades  
-----------------------------
  
Existem diversas funcionalidades novas no RMS com SP2:
  
-   [Melhor expansão de grupos em florestas](#bkmk_cif1)  
-   [Alterações no registo das bases de dados](#bkmk_cif2)  
-   [Maiores tamanhos de criação de batches em servidores](#bkmk_cif3)  
-   [Compatibilidade com o Microsoft SQL Server 2005](#bkmk_cif4)
  
<span id="BKMK_CIF1"></span>
#### Melhor expansão de grupos em florestas
  
#### O que faz esta funcionalidade?
  
No RMS, a expansão de grupos em florestas facilita a possibilidade de o RMS expandir a associação a um grupo Active Directory numa floresta diferente, em que as associações a um grupo não estão replicadas entre duas florestas. Quando um utilizador numa floresta envia conteúdo protegido para um utilizador noutra floresta, o RMS passa por um período de descoberta em que verifica se o utilizador tem acesso ao conteúdo. Este processo de verificação é efectuado com a utilização de uma consulta LDAP de uma floresta para a outra, de forma a encontrar o ponto de ligação do serviço (SCP) do RMS da floresta remota. Quando o SCP da floresta remota tiver sido descoberto, a conta de serviço do RMS envia um pedido para o pipeline de expansão de grupos. O pedido pergunta à floresta remota se um utilizador é um membro de um grupo.
  
#### A quem se aplica esta funcionalidade?
  
Esta nova funcionalidade terá interesse para os clientes RMS num ambiente Active Directory de múltiplas florestas, cujas associações a grupos universais não estão replicadas entre florestas.
  
#### Por que razão é importante esta alteração?
  
O novo protocolo de expansão de fidedignidade de floresta melhorará a fiabilidade para os clientes que estão a implementar um ambiente Active Directory de múltiplas florestas.
  
#### O que está diferente?
  
Anteriormente ao RMS com SP2, a expansão de grupos entre florestas era obtida através de chamadas remotas .NET. Nesta versão, o protocolo de expansão de grupos em florestas foi alterado para um serviço Web ASP.NET que utiliza pedidos SOAP/HTTP para o pipeline de expansão de grupos com fidedignidade de floresta.
  
| ![](images/Cc747637.note(WS.10).gif)Nota                                                                                                                                                                                                             |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Para fins de retro-compatibilidade, as chamadas remotas .NET ainda são suportadas no RMS com SP2. No entanto, para poder tirar o máximo partido do novo protocolo de expansão de grupos em florestas, todos os clusters do RMS devem estar a utilizar, pelo menos, o RMS com SP2. |
  
#### Que definições são adicionadas ou alteradas no RMS com SP2?
  
Por predefinição, o novo pipeline de expansão de grupos do RMS está configurado com as definições mais seguras no RMS com SP2, a que apenas o serviço do RMS local e os grupos de administradores têm acesso. Para dar acesso a uma conta, deve alterar a lista de controlo de acessos no pipeline de expansão de grupos, que se encontra em wwwroot\\\_wmcs\\GroupExpansion\\GroupExpansion.asmx.
  
| ![](images/Cc747637.Important(WS.10).gif)Importante                                                                                                                                                                                                                                                                                                                                                                    |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Assegure-se de que a conta do serviço do RMS em cada floresta do Active Directory tem acesso ao pipeline de expansão de grupos em cada servidor RMS no cluster. Se as contas não tiverem acesso, a expansão de grupos não será bem sucedida. Em alternativa, pode criar a mesma conta em cada floresta e atribuir a mesma palavra-passe a cada conta. Neste caso, apenas necessita de adicionar essa única conta ao pipeline de expansão de grupos. |
  
Foram adicionados novos eventos ao RMS com SP2 para o informar sobre mensagens com problemas que não entraram no serviço de Colocação de Mensagens em Fila. Estes novos registos de eventos incluem eventos que o notificam sempre que não seja possível assinar digitalmente uma mensagem ou não seja possível validar a mensagem. Alguns exemplos de problemas de validação incluem uma mensagem formada incorrectamente, a falta de um "hash" ou de uma assinatura, ou um "hash" ou uma assinatura incorrectos.
  
<span id="BKMK_CIF2"></span>
#### Alterações no registo das bases de dados
  
#### O que faz esta funcionalidade?
  
O RMS utiliza um serviço de escuta do registo que envia todas as comunicações do RMS para uma base de dados de registo utilizando a Colocação de Mensagens em Fila. O cluster do RMS submete mensagens ao serviço de Colocação de Mensagens em Fila e o serviço de escuta do registo recupera essas mensagens da fila da Colocação de Mensagens em Fila e escreve-as na base de dados de registo.
  
#### A quem se aplica esta funcionalidade?
  
Esta funcionalidade aplica-se aos actuais utilizadores do RMS que estão a utilizar o serviço de escuta do registo do RMS e aos novos utilizadores do RMS com SP2 que estão a considerar a utilização do serviço de escuta do registo do RMS.
  
#### Por que razão é importante esta alteração?
  
Nas versões anteriores do RMS, a fila de registo do RMS estava protegida utilizando listas de controlo de acesso, mas a autenticação não estava activada. Sem autenticação, um utilizador mal intencionado poderia potencialmente escrever mensagens erradas na fila de registo do RMS.
  
#### O que está diferente?
  
No RMS com SP2 existe uma autenticação adicional nas mensagens transmitidas pelo cluster do RMS utilizando a Colocação de Mensagens em Fila. Além das listas de controlo de acesso que evitam o acesso não autorizado à fila de mensagens, a fila do serviço de Colocação de Mensagens em Fila também está protegida utilizando um mecanismo de verificação da autenticidade da mensagem. Quando é enviada uma mensagem para o serviço de Colocação de Mensagens em Fila, os pipelines do RMS geram um "hash" da mensagem e assinam-na digitalmente utilizando a chave privada do cluster do RMS. O Serviço de Escuta do Registo calcula primeiro o seu próprio "hash" da mensagem e compara-o com o "hash" incluído na mensagem. Se os "hashes" corresponderem, o Serviço de Escuta do Registo verifica a assinatura utilizando a chave pública do cluster e o "hash" na mensagem. Se os "hashes" corresponderem e a assinatura for verificada, a mensagem é enviada para a base de dados de registo. Se os passos de validação não forem bem sucedidos, a mensagem será permanentemente apagada da fila do serviço de Colocação de Mensagens em Fila e será escrito um aviso de evento para o registo de aplicações no Visualizador de Eventos.
  
#### Que definições são adicionadas ou alteradas no RMS com SP2?
  
Foram adicionados novos eventos ao RMS com SP2 para o informar sobre mensagens com problemas que não entraram no serviço de Colocação de Mensagens em Fila. Estes novos eventos são escritos no registo de aplicações e incluem mensagens que não podem ser assinadas digitalmente ou assinaturas digitais na mensagem que não podem ser validadas. Alguns exemplos de problemas de validação incluem uma mensagem formada incorrectamente, a falta de um "hash" ou de uma assinatura, ou um "hash" ou uma assinatura incorrectos.
  
<span id="BKMK_CIF3"></span>
#### Maiores tamanhos de criação de batches em servidores
  
#### O que faz esta funcionalidade?
  
A criação de batches no RMS aumenta o desempenho, permitindo que sejam enviados múltiplos pedidos de licença para o cluster do RMS como um único pedido, em vez de fazer um pedido individual para cada licença.
  
#### A quem se aplica esta funcionalidade?
  
O suporte para tamanhos maiores de criação de batches em servidores será do interesse das aplicações activadas pelo RMS que necessitam de adquirir várias licenças para conteúdo protegido ao mesmo tempo.
  
#### Por que razão é importante esta alteração?
  
A utilização de batches do RMS permite que seja emitido um único pedido ao pipeline AcquireLicense do RMS para obter Licenças de utilização para múltiplos Certificados de Contas de Direitos (RACs) face a uma ou mais Licenças de Publicação. Sem um tamanho de batches superior a 1, a aplicação activada pelo RMS teria de pedir individualmente uma Licença de utilização para cada utilizador.
  
#### O que está diferente?
  
Nas versões do RMS anteriores ao RMS com SP2, o cluster do RMS suportava um tamanho máximo de batches de 1. Se o tamanho máximo estivesse definido para um número superior a 1, o cluster não o teria em consideração. No RMS com SP2, este tamanho de batches pode ascender a 100.
  
| ![](images/Cc747637.note(WS.10).gif)Nota         |  
|-------------------------------------------------------------------------------|  
| Apenas o pipeline AcquireLicense do RMS inclui suporte para pedidos em batch. |
  
O relatório de erros foi melhorado no RMS com SP2 para ter em conta pedidos em batch. Por exemplo, se enviar um batch de dez pedidos e o segundo e terceiro pedido falharem, será escrito um evento no registo de eventos para cada falha.
  
<span id="BKMK_CIF4"></span>
#### Compatibilidade com o Microsoft SQL Server 2005
  
#### O que faz esta funcionalidade?
  
No RMS com SP2, o Microsoft SQL Server 2005 pode ser utilizado como o servidor de base de dados para suportar as bases de dados de configuração e de registo do RMS, sem efectuar qualquer configuração adicional.
  
#### A quem se aplica esta funcionalidade?
  
O suporte para o Microsoft SQL Server 2005 com o RMS com SP2 será do interesse dos clientes RMS que pretendem utilizar o Microsoft SQL Server 2005 como a sua base de dados do RMS.
  
#### Por que razão é importante esta alteração?
  
Nas versões anteriores do RMS, os tipos de dados de alguns dos parâmetros utilizados na tabela sysmessages eram incompatíveis com a especificação de formato do Microsoft SQL Server 2005. Para mais informações, consulte o artigo 913372 da Base de Dados de Conhecimento da Microsoft ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)).
  
#### O que está diferente?
  
Nas versões do RMS anteriores ao RMS com SP2, eram utilizadas declarações SQL RAISERROR para notificar o utilizador do RMS de que tinha ocorrido um erro. A declaração RAISERROR consulta a tabela sysmessages para recuperar as mensagens de erro do RMS guardadas nesta tabela. O RMS com SP2 utiliza uma técnica diferente para propagar erros SQL, para que deixe de haver uma dependência da tabela sysmessages.
  
| ![](images/Cc747637.note(WS.10).gif)Nota                                                                                                                                                                                                                                                            |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Se estiver a actualizar do RMS com SP1 para o RMS com SP2, a tabela sysmessages já não é consultada para verificar a existência de mensagens de erro, mas as próprias mensagens de erro permanecerão na tabela sysmessages. Uma instalação de raiz do RMS com SP2 não adicionará quaisquer novas entradas na tabela sysmessages. |
  
Problemas conhecidos  
--------------------
  
As secções seguintes alertam para problemas conhecidos com esta versão do RMS.
  
#### O ficheiro de ajuda ainda faz referência ao RMS com Service Pack 1
  
O ficheiro de ajuda fornecido na instalação do RMS com SP2 ainda faz referência ao RMS com SP1. Para mais informações sobre o RMS com SP2, consulte as informações sobre Serviços de Gestão de Direitos ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)).
  
#### O Windows Update não instala o cliente RMS com SP2 em computadores baseados em x64 ou Itanium
  
Se o cliente RMS ou o cliente RMS com SP1 estiver instalado num computador baseado em x64 e se tentar actualizar para o cliente RMS com SP2 (x64) a partir do Windows Update, a instalação falha. Embora os anteriores clientes RMS, que foram criados para sistemas de 32 bits, funcionassem nos computadores baseados em x64, não podem ser actualizados para o cliente RMS com SP2 (x64). Primeiro é necessário desinstalar o cliente RMS anterior e iniciar novamente a actualização. O Windows Update detecta a versão do sistema operativo e fornece o cliente RMS com SP2 adequado. O mesmo acontece para os computadores baseados em Itanium.
  
#### O reaprovisionamento nunca inicia o serviço de escuta do registo
  
Quando o cluster não está aprovisionado, o serviço de escuta do registo não deixa o serviço em estado de paragem. Para parar totalmente o serviço, deve reiniciar o computador.
  
#### Não é possível remover um domínio de publicação fidedigno não baseado em software
  
Após importar um domínio de publicação fidedigno com uma implementação da chave privada não baseada em software, não é possível eliminá-lo. A importação de uma chave privada não baseada em software não pode ser feita a partir da consola de administração dos Serviços de Gestão de Direitos. Contacte o respectivo fornecedor do hardware para obter instruções sobre como exportar e importar a chave privada.
  
#### O Microsoft .NET Framework 2.0 muda as raízes virtuais do IIS quando instalado no servidor RMS
  
O RMS com SP2 utiliza o mapeamento de scripts do ASP.NET incluído no .NET Framework versão 1.1. O mapeamento fornecido pelas versões posteriores não é compatível com o RMS com SP2. No entanto, ambas as versões podem coexistir sem interferências com outras aplicações dependentes. Se o servidor tiver o .NET Framework 1.1 e o .NET Framework 2.0 ou posterior instalado, depois de a instalação e o aprovisionamento do RMS com SP2 parecerem ter sido concluídos com sucesso, o cluster do RMS pode não funcionar correctamente. O motivo para esta situação é que as raízes virtuais do RMS necessitam de ser registadas no mapa de script do ASP.NET versão 1.1 em vez da versão 2.0. Para registar as raízes virtuais do RMS com o mapa de script do ASP.NET versão 1.1, execute o seguinte comando numa linha de comandos:
  
**%windir%\\Microsoft.NET\\Framework\\v1.1.4322&gt;aspnet\_regiis.exe -s W3SVC/1/ROOT/\_wmcs**
  
Executar este comando registará adequadamente as raízes virtuais do RMS e permitirá que o RMS com SP2 seja executado no servidor.
  
#### A associação a grupos poderá não existir se utilizar o Active Directory no nível funcional do modo nativo do Windows 2000
  
Quando implementar o RMS num ambiente em que os níveis de infra-estrutura do RMS foram elevados para o nível funcional do modo nativo do Windows 2000, o RMS pode não ler o atributo memberOf dos objectos Active Directory quando tentar expandir as listas de distribuição da associação a grupos que estão ocultas. Para permitir que o RMS leia o atributo memberOf, a conta de Serviço do RMS deverá utilizar uma conta de domínio que seja membro do grupo de pré-acesso compatível com o Windows 2000. Para mais informações, consulte o artigo 812841 da Base de Dados de Conhecimento da Microsoft ([http://go.microsoft.com/fwlink/?LinkId=78152](http://go.microsoft.com/fwlink/?linkid=78152)).
  
#### O serviço de escuta do registo envia mensagens de Colocação de Mensagens em Fila para a fila de mensagens não entregues quando a base de dados não está acessível
  
Existem casos (por exemplo, a base de dados está indisponível, problemas de conectividade de rede, entre outros) em que o serviço de escuta do registo não pode aceder à base de dados. Neste caso, as mensagens são enviadas para uma fila de mensagens não entregues. A única forma de recuperar estas mensagens (ou seja, enviá-las para a base de dados de registo) é utilizar a ferramenta RMS Queue Recovery fornecida com o RMS Administration Toolkit. Para transferir o RMS Administration Toolkit, consulte [http://go.microsoft.com/fwlink/?LinkId=33841](http://go.microsoft.com/fwlink/?linkid=33841).
  
| ![](images/Cc747637.note(WS.10).gif)Nota                                                                                                                                                                                                  |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Os comandos Recover e RecoverandPurge foram removidos de LogRecoveryCmd. Isto garante que todas as mensagens são reencaminhadas através do serviço de Colocação de Mensagens em Fila e autenticadas antes que a mensagem seja enviada para a base de dados de registo. |
  
#### Deve actualizar o RMS com SP2 antes de actualizar o Microsoft SQL Server 2005
  
Quando actualizar para o RMS com SP2 e do Microsoft SQL Server 2000 para o Microsoft SQL Server 2005, certifique-se de que actualiza primeiro o RMS. Isto evitará quaisquer problemas de compatibilidade com a actualização do Microsoft SQL Server.
  
#### O RMS com SP2 não aprovisiona em Web sites cujo nome inclui um apóstrofo (')
  
Se tentar aprovisionar o RMS com SP2 num Web site cujo nome inclua um apóstrofo ('), o processo de aprovisionamento falhará e apresentará uma mensagem de erro de **Parâmetro inválido**. Para aprovisionar o RMS com SP2 no Web site, retire o apóstrofo do nome do Web site.
  
#### Activar o ASP.NET versão 1.1 nos servidores com uma versão de 64 bits do Windows Server 2003
  
O tópico "Requisitos do sistema" na Ajuda do RMS explica como instalar o .NET Framework 1.1 e activar o ASP.NET 1.1 depois de instalar os Serviços de Informação Internet (IIS). No entanto, se o .NET Framework 1.1 for instalado antes do IIS, o ASP.NET 1.1 não será apresentado nas extensões do serviço Web e o procedimento documentado não será útil. Se o IIS for instalado depois de instalar o .NET Framework 1.1, execute o comando seguinte numa linha de comandos para activar o ASP.NET:
  
**%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis.exe -i –enable**
  
Quando utilizar uma versão do .NET Framework posterior à  1.1, substitua o **-i** por **-ir** neste comando para evitar reiniciar quaisquer mapas existentes do script IIS.
  
#### A conta do serviço do RMS da floresta remota deve ser adicionada ao pipeline local groupexpansion
  
Foi corrigido um problema de segurança que remove BUILTIN\\users do ACL no pipeline groupexpansion. Tal pode interromper a expansão de grupos em cenários de florestas. Para resolver este problema, siga os seguintes passos:
  
**Adicione uma conta do serviço do RMS à floresta remota**  
1.  Em Floresta1, em que Floresta1 é o cluster de raiz do RMS na primeira floresta, aceda a inetpub\\wwwroot\\\_wmcs.
  
2.  Clique com o botão direito do rato na pasta **GroupExpansion** e seleccione **Propriedades**.
  
3.  Na janela de **Propriedades GroupExpansion** clique no separador de **Segurança** e adicione a entrada para *Floresta2\\ContaServiçoRMS* (por exemplo, rmil31\\rmsvc), em que Floresta2 é o cluster de raiz do RMS na segunda floresta.
  
4.  Clique em **OK**.
  
5.  Clique em **Executar**, escreva **iisreset** e clique em**OK**.
  
#### Actualizar o .NET Framework pode resultar na perda de dados
  
Se o .NET Framework (CLR) versão 1.1 for actualizado após o RMS ter sido instalado e aprovisionado, as raízes virtuais (vroots) estarão definidas para utilizar o .NET Framework versão 2.0. Se isto acontecer, não são registadas quaisquer informações na base de dados de registo. Isto resultará na perda de dados. Efectue uma das seguintes acções:
  
-   Actualize o .NET Framework antes de instalar e aprovisionar o RMS.  
-   Reinicie as raízes virtuais (vroots) para utilizar a versão 1.1 após a actualização do .NET Framework.
  
Alterações à documentação neste lançamento  
------------------------------------------
  
Aqui está uma lista de tópicos que foram alterados nesta versão:
  
-   Considerar Fidedignos os Certificados de Contas Baseados no Passport ([http://go.microsoft.com/fwlink/?LinkId=70369](http://go.microsoft.com/fwlink/?linkid=70369))  
-   Requisitos de Software para o RMS ([http://go.microsoft.com/fwlink/?LinkId=70371](http://go.microsoft.com/fwlink/?linkid=70371))  
-   Como Implementar clientes RMS ([http://go.microsoft.com/fwlink/?LinkId=70373](http://go.microsoft.com/fwlink/?linkid=70373))  
-   Instalação do RMS a partir da Linha de Comandos ([http://go.microsoft.com/fwlink/?LinkId=70374](http://go.microsoft.com/fwlink/?linkid=70374))  
-   Tabelas Essenciais à Base de Dados de Configuração do RMS ([http://go.microsoft.com/fwlink/?LinkId=70375](http://go.microsoft.com/fwlink/?linkid=70375))  
-   Tabelas de Certificação da Base de Dados de Configuração do RMS ([http://go.microsoft.com/fwlink/?LinkId=70376](http://go.microsoft.com/fwlink/?linkid=70376))  
-   Tabelas de Bases de Dados de Registo do RMS ([http://go.microsoft.com/fwlink/?LinkId=70377](http://go.microsoft.com/fwlink/?linkid=70377))  
-   Avaliar Requisitos de Escalabilidade [http://go.microsoft.com/fwlink/?LinkId=70378](http://go.microsoft.com/fwlink/?linkid=70378))  
-   Proteger a Implementação do RMS ([http://go.microsoft.com/fwlink/?LinkId=70379](http://go.microsoft.com/fwlink/?linkid=70379))  
-   Activar o Serviço de Desactivação ([http://go.microsoft.com/fwlink/?LinkId=70380](http://go.microsoft.com/fwlink/?linkid=70380))  
-   Planeamento para Utilizadores Externos do RMS [http://go.microsoft.com/fwlink/?LinkId=70381](http://go.microsoft.com/fwlink/?linkid=70381))  
-   Activar o Suporte do Servidor RMS para Dispositivos Móveis e Serviços de Servidor ([http://go.microsoft.com/fwlink/?LinkId=70382](http://go.microsoft.com/fwlink/?linkid=70382))
  
#### Copyright
  
*As informações contidas neste documento representam a visão actual da Microsoft Corporation sobre os problemas discutidos na data de publicação. Como a Microsoft tem de responder a condições de mercado em constante mutação, não deverá ser interpretado como um compromisso da parte da Microsoft, e a Microsoft não pode garantir a precisão de qualquer informação apresentada a partir da data de publicação.*
  
*Este documento destina-se apenas a fins informativos. A MICROSOFT NÃO FORNECE QUALQUER GARANTIA, EXPRESSA, IMPLÍCITA OU LEGAL, ÀS INFORMAÇÕES DESTE DOCUMENTO.*
  
*É da responsabilidade do utilizador o cumprimento das leis de direitos de autor aplicáveis. Sem limitação dos direitos protegidos por copyright, nenhuma parte deste documento pode ser reproduzida, guardada ou introduzida em sistemas de dados, ou transmitida por qualquer forma ou meio (electrónico, mecânico, fotocópia, gravação ou outro), nem para quaisquer fins, sem o consentimento expresso, por escrito, da Microsoft Corporation.*
  
*A Microsoft pode ter patentes, pedidos de patentes, marcas comerciais, copyrights e outros direitos de propriedade intelectual sobre a matéria tratada neste documento. Salvo disposição expressa em qualquer contrato de licença escrito da Microsoft, o facto de este documento lhe ser fornecido não lhe concede quaisquer direitos ou licenças sobre essas patentes, marcas comerciais, direitos de autor ou outro tipo de propriedade intelectual.*
  
*Salvo indicação em contrário, os exemplos de empresas, organizações, produtos, nomes de domínio, endereços de correio electrónico, logótipos, pessoas, lugares e eventos aqui apresentados são fictícios e não são intencionais nem devem inferir-se quaisquer associações a qualquer empresa, organização, produto, nome de domínio, endereço de correio electrónico, logótipo, pessoa, lugar ou evento real.*
  
*© 2006 Microsoft Corporation. Todos os direitos reservados.*
  
*Active Directory, Microsoft, MS-DOS, Visual Studio, Windows, Windows Server, SQL Server e Windows NT são marcas registadas ou marcas comerciais da Microsoft Corporation nos Estados Unidos e/ou noutros países.*
  
*Os nomes de empresas e produtos reais mencionados neste documento podem ser marcas comerciais dos respectivos proprietários.*
