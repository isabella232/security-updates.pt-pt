---
TOCTitle: Definições de Chave do RMS
Title: Definições de Chave do RMS
ms:assetid: 'b052305c-1db7-434a-bad9-26d704156776'
ms:contentKeyID: 18124129
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747729(v=WS.10)'
---

Definições de Chave do RMS
==========================

A tabela seguinte lista as chaves que são utilizadas num sistema do RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Chave</th>
<th>Utilização</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Chaves de servidor</td>
<td style="border:1px solid black;"><strong>Chave pública</strong>
Encripta a chave de conteúdo de uma licença de publicação para que apenas o servidor do RMS possa obter a chave de conteúdo e emitir as licenças de utilização para essa licença de publicação.
<strong>Chave privada</strong>
Assina todos os certificados e licenças emitidos pelo servidor.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Chaves de máquinas</td>
<td style="border:1px solid black;"><strong>Chave pública</strong>
Encripta uma chave privada do certificado de conta de direitos.
<strong>Chave privada</strong>
Desencripta um certificado de conta de direitos.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Chaves de licenciador de clientes</td>
<td style="border:1px solid black;"><strong>Chave pública</strong>
Encripta a chave de conteúdo simétrica nas licenças de publicação que emite.
<strong>Chave privada</strong>
Assina licenças de publicação que são emitidas localmente quando o utilizador não está ligado à rede.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Chaves de utilizador</td>
<td style="border:1px solid black;"><strong>Chave pública</strong>
Encripta a chave de conteúdo de uma licença de utilização para que um utilizador específico possa consumir conteúdo protegido pelo RMS através dessa licença.
<strong>Chave privada</strong>
Permite ao utilizador consumir conteúdo protegido pelo RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Chaves de conteúdo</td>
<td style="border:1px solid black;">Encripta o conteúdo protegido pelo RMS quando o autor o publica.</td>
</tr>
</tbody>
</table>
