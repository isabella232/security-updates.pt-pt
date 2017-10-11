---
TOCTitle: Instalação do Servidor do RMS a partir da Linha de Comandos
Title: Instalação do Servidor do RMS a partir da Linha de Comandos
ms:assetid: 'b55b1e2a-dd14-4168-a37f-9cdedbec660b'
ms:contentKeyID: 18124130
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747733(v=WS.10)'
---

Instalação do Servidor do RMS a partir da Linha de Comandos
===========================================================

Pode instalar o RMS com Service Pack 2 (SP2) a partir da linha de comandos, o que lhe permite automatizar a instalação. A automatização da instalação pode ser efectuada através de uma das duas formas que se seguem: efectuar uma instalação automática utilizando o cliente EXE transferido ou utilizar os ficheiros MSI extraídos a partir do EXE transferido para instalar o cliente RMS. Para instalar utilizando o ficheiro EXE transferido, utilize a sintaxe seguinte:

**WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q**

Para instalar utilizando os ficheiros do Windows® Installer (.msi), deve primeiro extrair os ficheiros msi do ficheiro executável do RMS com SP2. O comando seguinte pode ser executado a partir de uma linha de comandos para extrair os ficheiros msdrmclient.msi e RmClientBackCompat.msi:

**WindowsRightsManagementServiceSP2-KB917275-Server-ENU.exe /X:C:\\***Install\_Location*

Após a extracção dos ficheiros .msi, pode utilizar os comandos seguintes para instalar o RMS:

**msiexec.exe /I MSDrmClient.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Install\_Location*

**msiexec.exe /I RMClientBackCompat.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Install\_Location*

A tabela seguinte descreve a sintaxe para cada comando.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parâmetro</th>
<th>Definição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/I MSDrmClient.msi</strong> ou <strong>/I RMClientBackCompat.msi</strong></td>
<td style="border:1px solid black;">Necessário. Especifica o produto a ser instalado.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/qn</strong></td>
<td style="border:1px solid black;">Opcional. Especifica uma instalação sem a interacção do utilizador.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/lei</strong> <em>logfile.log</em></td>
<td style="border:1px solid black;">Opcional. Especifica o ficheiro em que devem ser registadas as mensagens de erro e de estado.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>DISPLAYPAGE=”NO”</strong></td>
<td style="border:1px solid black;">Opcional. Especifica que a página <strong>Administração Global</strong> não será apresentada após a instalação.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>TARGETDIR=c:\</strong><em>Install_Location</em></td>
<td style="border:1px solid black;">Opcional. Especifica o directório de instalação do RMS com Service Pack 2. Se não especificar uma localização, será utilizada a localização de instalação predefinida.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747733.note(WS.10).gif)Nota                                                                                                                                                                                                 |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Independentemente do método de instalação escolhido para a implementação, deve certificar-se de que ambos os ficheiros .msi são instalados com êxito. Se ocorrer um erro que impeça a instalação do MSDrmClient.msi, o RMClientBackCompat.msi não deve ser instalado. |
