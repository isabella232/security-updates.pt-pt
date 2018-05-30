---
TOCTitle: Serviço de Licenciamento do RMS
Title: Serviço de Licenciamento do RMS
ms:assetid: '5cad1baf-0304-4e82-b62d-83a4aac2140b'
ms:contentKeyID: 18123999
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720278(v=WS.10)'
---

Serviço de Licenciamento do RMS
===============================

O serviço de licenciamento, que emite licenças de utilização, é executado no cluster de raiz do RMS e nos clusters de licenciamento. As licenças de utilização permitem aos utilizadores consumirem conteúdo protegido.

O ficheiro da aplicação do serviço de licenciamento, License.asmx, encontra-se no directório virtual Licensing que está no IIS.

| ![](/security-updates/images/Cc720278.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                                                                                       |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pode implementar um cluster de licenciamento à parte para descarregar os pedidos de licenciamento provenientes do cluster de raiz. Também pode implementar um servidor ou um cluster à parte para um departamento, por exemplo, para que esse departamento possa estabelecer as suas próprias políticas de direitos. Para mais informações sobre estas considerações, veja como identificar os componentes principais em "RMS: Planeamento e Arquitectura", nesta colecção de documentação. |

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
