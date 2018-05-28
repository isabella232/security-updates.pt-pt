---
TOCTitle: Suporte dos Serviços de Informação Internet para o RMS
Title: Suporte dos Serviços de Informação Internet para o RMS
ms:assetid: 'bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c'
ms:contentKeyID: 18124160
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747649(v=WS.10)'
---

Suporte dos Serviços de Informação Internet para o RMS
======================================================

Os serviços primários do RMS são fornecidos por um conjunto de serviços Web do ASP .NET. Esses serviços Web são executados nos Serviços de Informação Internet (IIS) da Microsoft®. Durante o processo de aprovisionamento do servidor, o RMS configura os directórios virtuais no IIS. Os ficheiros de aplicações para os serviços Web são instalados em directórios virtuais.

Durante o aprovisionamento de servidores, pode seleccionar o Web site sob o qual pretende definir directórios virtuais a partir de uma lista de Web sites que existem no servidor. Antes de aprovisionar um servidor, pode criar um Web site especial para o RMS. Se o fizer, pode configurar as restrições de autenticação e de acesso específicas da implementação do RMS.

Por predefinição, os ficheiros dos serviços Web e os directórios virtuais são protegidos por listas de controlo de acesso discricionário (DACL) para impedir o acesso não autorizado às respectivas funcionalidades. As entradas de controlo de acesso (ACE) destes itens são as seguintes:

-   O grupo de administradores tem controlo total
-   O sistema local tem controlo total
-   O RMS Service Group tem permissões de Leitura e de Execução
-   Convidados e Utilizadores têm permissões de Leitura e Execução, Listagem do Conteúdo das Pastas e Leitura
-   O acesso anónimo não é permitido

A tabela seguinte apresenta uma lista dos directórios virtuais que são criados no IIS, bem como dos serviços que são instalados nesses directórios.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Directório virtual</th>
<th>Serviço</th>
<th>Ficheiro do serviço Web</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">_wmcs</td>
<td style="border:1px solid black;">Este é o directório virtual da administração do cluster do RMS</td>
<td style="border:1px solid black;">Não aplicável</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certification</td>
<td style="border:1px solid black;">Este directório virtual contém os serviços que suportam a certificação do RMS</td>
<td style="border:1px solid black;">Não aplicável</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Proxy de activação</td>
<td style="border:1px solid black;">Activation.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certificação de contas</td>
<td style="border:1px solid black;">Certification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Pré-certificação</td>
<td style="border:1px solid black;">Precertification.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Serviço de localizador</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Servidor</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certificação de Servidor</td>
<td style="border:1px solid black;">ServerCertification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certificação de Dispositivo Móvel</td>
<td style="border:1px solid black;">MobileDeviceCertfication.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Inscrição</td>
<td style="border:1px solid black;">SubEnrollService.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licenciamento</td>
<td style="border:1px solid black;">Este directório virtual contém os serviços que suportam o licenciamento do RMS</td>
<td style="border:1px solid black;">Não aplicável</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Licenciamento</td>
<td style="border:1px solid black;">License.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Publicação</td>
<td style="border:1px solid black;">Publish.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Servidor</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Serviço de localizador</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Admin</td>
<td style="border:1px solid black;">Este directório virtual contém os serviços que suportam a administração do RMS</td>
<td style="border:1px solid black;">Não aplicável</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Administração</td>
<td style="border:1px solid black;">AdminSvc.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">Interface .NET Remoting</td>
<td style="border:1px solid black;">Não aplicável</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DirectoryServices</td>
<td style="border:1px solid black;">Subdirectório de DrmRemote</td>
<td style="border:1px solid black;">Não aplicável</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc747649.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| O serviço de Administração tem maiores restrições do que os outros serviços Web, uma vez que as interfaces fornecidas permitem configurar o RMS. Por este motivo, os membros do grupo de utilizadores não podem ter acesso ao serviço de Administração. Além disso, a filtragem de IP está activada a fim de garantir o acesso apenas ao computador local. O directório virtual DirectoryServices não dá acesso a utilizadores Convidados. O serviço Localizador de Serviços também concede um controlo total à conta de Serviço de Rede. Para aprovisionar um servidor de licenciamento, tem de alterar as ACEs predefinidas para permitir o acesso ao administrador do RMS. |
