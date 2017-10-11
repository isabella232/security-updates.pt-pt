---
TOCTitle: Requisitos de Software para o RMS
Title: Requisitos de Software para o RMS
ms:assetid: '17faf2ad-2366-4a92-98a5-766e20a0f741'
ms:contentKeyID: 18123906
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720201(v=WS.10)'
---

Requisitos de Software para o RMS
=================================

Os requisitos de software para executar servidores do RMS são apresentados na tabela seguinte.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Software</th>
<th>Requisito</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Sistema operativo</td>
<td style="border:1px solid black;">Qualquer edição do Microsoft Windows Server® 2003, excepto a Web Edition.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sistema de ficheiros</td>
<td style="border:1px solid black;">É recomendado o sistema de ficheiros NTFS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Componentes do sistema operativo</td>
<td style="border:1px solid black;"><ul>
<li>Colocação de Mensagens em Fila (também conhecida por MSMQ) com a Integração de Serviços de Directório do Active Directory® activada.<br />
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
<tr class="even">
<td style="border:1px solid black;">Serviço de directório do Active Directory®</td>
<td style="border:1px solid black;">O RMS tem de ser instalado num domínio do Active Directory no qual os controladores de domínio executam o Windows Server 2000 com o Service Pack 3 (SP3) ou posterior. Todos os utilizadores e grupos que utilizam o RMS para consumir e publicar conteúdos deverão ter um endereço de correio electrónico configurado no Active Directory.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Servidor da base de dados</td>
<td style="border:1px solid black;">O RMS necessita de uma base de dados e de procedimentos de armazenamento para efectuar as operações. Pode utilizar o Microsoft SQL Server 2000 com SP3a ou posterior, ou o Microsoft SQL Server 2005. Para fins de teste ou outras implementações em computadores individuais, é possível utilizar o Microsoft SQL Server Desktop Engine (MSDE 2000) com SP3 ou o Microsoft SQL Server 2005 Express Edition.</td>
</tr>
</tbody>
</table>
  
Se estiver a implementar o RMS num ambiente em que existem múltiplas florestas do Active Directory, deve utilizar os Grupos Universais do Active Directory para que a associação a grupos seja replicada em todos os Catálogos Globais. Para criar Grupos Universais, o nível funcional do seu domínio deve ser definido para, pelo menos, o nível nativo do Windows 2000 e o nível funcional da floresta deve ser elevado para o Windows Server 2003.
  
Recomenda-se a utilização do MSDE 2000 ou do Microsoft SQL Server 2005 Express Edition para suportar bases de dados do RMS apenas nos ambientes de teste, uma vez que o MSDE 2000 ou o Microsoft SQL Server 2005 Express Edition não suportam quaisquer interfaces de rede. Além disso, os termos de utilização para o MSDE 2000 ou o Microsoft SQL Server 2005 Express Edition especificam que não pode utilizar as ferramentas de cliente do SQL Server para manipular uma base de dados do MSDE 2000 ou do Microsoft SQL Server 2005 Express Edition. Com esta restrição não é possível ver informações relativas ao registo nem alterar dados armazenados na base de dados de configuração.
  
Se não tiver o ASP.NET versão 1.1 instalado no servidor, o processo de instalação depende se estiver a executar a versão de 32 bits do Windows Server 2003 ou a versão de 64 bits do Windows Server 2003.
  
Se estiver a executar a versão de 32 bits do Windows Server 2003, efectue estes passos para instalar e activar o ASP.NET versão 1.1:
  
1.  Abra **Adicionar ou Remover Programas** no **Painel de Controlo** e, em seguida, clique em **Adicionar/Remover Componentes do Windows**.  
2.  Clique em **Servidor de aplicações** e, em seguida, clique em **Detalhes**.  
3.  No Assistente Componentes do Windows, seleccione **ASP.NET**.  
4.  Se o ASP.NET 1.1 estiver instalado, mas não autorizado como uma extensão do serviço Web do IIS:  
    -   Abra o Gestor de Serviços de Informação Internet.  
    -   Clique em **Extensão do serviço Web do IIS**, seleccione ASP.NET v1.1.4322 e clique em **Permitir**.
  
Se estiver a executar a versão de 64 bits do Windows Server 2003, siga estes passos para instalar e activar o ASP.NET versão 1.1:
  
1.  Instale o .NET Framework 1.1, que instalará o ASP.NET 1.1. Pode transferir o Microsoft .NET Framework Version 1.1 Redistributable Package a partir do Centro de Transferências da Microsoft ([http://go.microsoft.com/fwlink/?LinkId=69985](http://go.microsoft.com/fwlink/?linkid=69985)).  
2.  Abra o Gestor de Serviços de Informação Internet.  
3.  Clique em Extensão do serviço Web do IIS, seleccione ASP.NET v1.1.4322 e clique em Permitir.
  
Se estiver a executar o RMS numa versão de 64 bits do Windows Server 2003, deverá utilizar os seguintes passos para activar o IIS para trabalhar com o RMS:
  
1.  Clique em **Iniciar** e, em seguida, clique em **Executar**.  
2.  Em **Abrir**, digite o seguinte comando e prima ENTER:
  
**"cscript %SystemDrive%\\inetpub\\AdminScripts\\adsutil.vbs set w3svc/AppPools/Enable32bitAppOnWin64 1"**
  
O RMS não foi concebido para o .NET Framework versão 2.0. Embora seja suportada uma instalação lado a lado, deve certificar-se de que o ASP.NET está configurado para utilizar o ASP.NET v1.1.4322. Dispõe de duas opções para se certificar de que uma instalação lado a lado é efectuada com êxito:
  
-   Certifique-se de que instala o .NET Framework versão 2.0 antes de instalar o servidor do RMS.  
-   Defina a versão do ASP.NET para a versão 1.1.4322 no Web site Predefinido no IIS utilizando o comando seguinte:
  
**"%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis -s w3svc/1/root"**
  
Para mais informações sobre o Active Directory, a Colocação de Mensagens em Fila e o IIS, consulte o Centro de Ajuda e Suporte do Windows Server 2003.
  
| ![](images/Cc720201.Caution(WS.10).gif)Atenção                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Pode aprovisionar o servidor do RMS no Web Site Predefinido ou em qualquer site que tenha sido anteriormente definido no IIS. Por motivos de segurança, este servidor não deve ser utilizado para executar outros sites ou serviços. Se for, isso poderá ter como resultado que várias aplicações e serviços sejam executados sob a mesma conta que o RMS (especialmente a conta de Sistema Local), o que pode fazer com que as chaves privadas fiquem expostas a operações sem garantias. Não deve aprovisionar o servidor do RMS no mesmo Web site que o Microsoft Office SharePoint Server 2007. Não é possível utilizar o RMS com autenticação Kerberos. O aprovisionamento do servidor do RMS num Web site desactiva a autenticação Kerberos desse servidor. Se o RMS não estiver configurado para utilizar o ASP.NET v1.1.4322, não será registada qualquer informação na base de dados de registo, o que resultará na perda de dados. |
  
Consulte Também  
---------------
  
####  
  
[Planear a Infra-estrutura de Servidores de Bases de Dados](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
