---
TOCTitle: Base de Dados de Serviços de Directório do RMS
Title: Base de Dados de Serviços de Directório do RMS
ms:assetid: '6f6b8586-5d17-4a40-94a3-4dc738195301'
ms:contentKeyID: 18124045
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747617(v=WS.10)'
---

Base de Dados de Serviços de Directório do RMS
==============================================

O servidor de bases de dados aloja a base de dados de serviços de directório que contém informações sobre utilizadores, identificadores (tais como endereços de correio electrónico), ID de segurança (SID), membros de grupos e identificadores alternativos. Estas informações são obtidas através de consultas LDAP efectuadas no catálogo global do Active Directory pelo serviço de Licenciamento do RMS. Para mais informações sobre este processo e os respectivos objectivos, consulte "[Cache do Active Directory do RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)" posteriormente nesta secção.

O RMS Service Group possui permissões de Execução nos procedimentos armazenados que estão na base de dados de serviços de directório.

A tabela seguinte mostra os atributos do Active Directory que estão armazenados nas tabelas da base de dados de serviços de directório.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Tabela</th>
<th>Atributo</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GroupAliases</td>
<td style="border:1px solid black;"><ul>
<li>GroupName: o alias para o grupo<br />
<br />
</li>
<li>GroupID: o ID exclusivo para este grupo<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>GroupDN: o nome distinto do Active Directory para este grupo<br />
<br />
</li>
<li>GroupID: o ID exclusivo para este grupo<br />
<br />
</li>
<li>Expiration: a data e hora em que expiram as informações guardadas para este grupo<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembership</td>
<td style="border:1px solid black;"><ul>
<li>GroupID: o ID exclusivo para este grupo<br />
<br />
</li>
<li>ParentID: o ID exclusivo para o grupo do qual este grupo é um membro<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalAliases</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalName: um nome de alias para o principal<br />
<br />
</li>
<li>PrincipalID: o ID exclusivo para este principal<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PrincipalIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalID: o ID exclusivo para este principal<br />
<br />
</li>
<li>Expiration: a data e hora em que expiram as informações guardadas para este principal<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalMembership</td>
<td style="border:1px solid black;">Cada fila desta tabela inclui o ID exclusivo de um principal e o ID exclusivo do grupo do qual é membro.
<ul>
<li>PrincipalID: o ID exclusivo para este principal<br />
<br />
</li>
<li>ParentID: o ID exclusivo de um grupo do qual este principal é um membro<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
