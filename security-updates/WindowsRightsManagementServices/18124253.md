---
TOCTitle: Serviço de Certificação de Contas do RMS
Title: Serviço de Certificação de Contas do RMS
ms:assetid: 'fb294969-850e-44b4-8f6a-ca5d5cec1bf1'
ms:contentKeyID: 18124253
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747802(v=WS.10)'
---

Serviço de Certificação de Contas do RMS
========================================

O serviço de certificação de contas apenas é executado no cluster de raiz. O serviço de certificação de contas cria certificados de contas de direitos que associam as contas de utilizador a computadores específicos. Um certificado de conta de direitos permite a um utilizador publicar ou consumir o conteúdo protegido quando utiliza um computador específico.

O ficheiro da aplicação do serviço de certificação de contas, Certification.asmx, encontra-se no directório virtual Certification que está no IIS.

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
