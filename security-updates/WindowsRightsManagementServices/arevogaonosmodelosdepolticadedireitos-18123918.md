---
TOCTitle: A Revogação nos Modelos de Política de Direitos
Title: A Revogação nos Modelos de Política de Direitos
ms:assetid: '287c5b92-fcb5-4295-9c2b-4e37e643beb2'
ms:contentKeyID: 18123918
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720226(v=WS.10)'
---

A Revogação nos Modelos de Política de Direitos
===============================================

As condições de revogação são especificadas nos modelos de política de direitos. Os valores das condições de revogação escritas num modelo de política de direitos são capturados numa etiqueta de XrML REFRESH na licença de publicação que é emitida segundo esse modelo. A resultante licença de utilização que é emitida pelo servidor também contém a etiqueta REFRESH.

A tabela seguinte apresenta os parâmetros existentes na etiqueta REFRESH.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parâmetro</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">O ID da lista de revogações.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ADDRESS</td>
<td style="border:1px solid black;">O URL ou o caminho UNC onde as listas de revogações podem ser obtidas.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">A chave pública do emissor da lista de revogações. Esta chave pública corresponde à chave privada que foi utilizada para assinar a lista de revogações.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">INTERVALTIME</td>
<td style="border:1px solid black;">A duração máxima da lista de revogações, em dias. Se a lista de revogações em cache for mais antiga do que o permitido por INTERVALTIME, o cliente do RMS obtém a lista de revogações mais recente a partir do URL listado em ADDRESS. Isto garante que seja sempre utilizada uma lista de revogações actualizada.</td>
</tr>
</tbody>
</table>
  
Para mais informações sobre como criar modelos de política de direitos, consulte "Criar e Modificar Modelos de Política de Direitos" em "Utilizar um Servidor do RMS" nesta colecção de documentação.
