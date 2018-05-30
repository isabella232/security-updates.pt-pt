---
TOCTitle: Alterar as Definições da Cache do Active Directory
Title: Alterar as Definições da Cache do Active Directory
ms:assetid: '8789a7a5-2065-4fae-9104-e0a70f1f2fb6'
ms:contentKeyID: 18124085
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747586(v=WS.10)'
---

Alterar as Definições da Cache do Active Directory
==================================================

As definições no registo especificam o número de entradas que serão armazenadas na cache do Active Directory. Para melhorar o tempo de resposta aos pedidos de clientes, pode modificar essas definições. Para mais informações, consulte "Optimizar o Desempenho dos Serviços de Directório" anteriormente nesta secção. Também pode especificar o período de validade das informações que estão armazenadas na cache.

Em computadores com a versão de 32 bits do Windows Server 2003, a chave de registo seguinte é o caminho completo da subchave de registo das entradas de cache:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Em computadores com a versão de 64 bits do Windows Server 2003, a chave de registo seguinte é o caminho completo da subchave de registo das entradas de cache:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0\\DirectoryServices**

A tabela seguinte mostra as entradas que controlam o comportamento da cache de memória incorporada.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Tipo</th>
<th>Valor Predefinido</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrincipalCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Número máximo de principais e respectivos endereços de correio electrónico e SID que podem ser armazenados na cache.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Período de validade das informações em cache para os principais.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupIDCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Número máximo de grupos e respectivos endereços de correio electrónico e SID que podem ser armazenados na cache.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIDCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Período de validade das informações em cache para membros do grupo.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembershipCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Número máximo de contactos que são membros de um grupo e que podem ser armazenados na cache.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupMembershipCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Período de validade das informações em cache relativas aos contactos que são membros de um grupo.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc747586.Caution(WS.10).gif)Atenção                                                                                                                  |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Uma edição incorrecta do registo pode danificar gravemente o sistema. Antes de proceder a alterações do registo, faça uma cópia de segurança dos dados importantes que guarda no computador. |
  
| ![](/security-updates/images/Cc747586.note(WS.10).gif)Nota                                                                                                                                                                                                                                                        |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| As entradas de registo **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** e **ContactMembersofGroupCacheExpireMinutes** também controlam a expiração da cache na cache do Active Directory local na base de dados de serviços de directório no servidor da base de dados. |
