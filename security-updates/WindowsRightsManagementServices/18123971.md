---
TOCTitle: Serviço de Publicação do RMS
Title: Serviço de Publicação do RMS
ms:assetid: '4c0c8fe3-695c-4b2c-a2d3-cab9b52bbb25'
ms:contentKeyID: 18123971
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720267(v=WS.10)'
---

Serviço de Publicação do RMS
============================

O serviço de publicação, que emite licenças de publicação, é executado no cluster de raiz do RMS e nos clusters de licenciamento. As licenças de publicação definem a política sob a qual as licenças de utilização podem ser entregues.

O ficheiro da aplicação do serviço de publicação, Publish.asmx, encontra-se no directório virtual Licensing que está no IIS.

A lista de controlo de acessos predefinida neste serviço é apresentada na tabela seguinte:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Utilizador ou Grupo</th>
<th>Permissão predefinida</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Administradores</td>
<td style="border:1px solid black;">Controlo total</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Grupo de Serviços do RMS</td>
<td style="border:1px solid black;">Ler e executar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SISTEMA</td>
<td style="border:1px solid black;">Controlo total</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Utilizadores</td>
<td style="border:1px solid black;">Ler e executar</td>
</tr>
</tbody>
</table>
