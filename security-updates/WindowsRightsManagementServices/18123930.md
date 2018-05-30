---
TOCTitle: 'Serviço de Pré-certificação do RMS'
Title: 'Serviço de Pré-certificação do RMS'
ms:assetid: '09957294-167f-4f98-88e9-ae90fbeb26c1'
ms:contentKeyID: 18123930
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720191(v=WS.10)'
---

Serviço de Pré-certificação do RMS
==================================

O serviço de pré-certificação só é executado no cluster de raiz do RMS. Este serviço permite a um servidor pedir um certificado de conta de direitos em nome de um utilizador e pode ser utilizado para desenvolver aplicações personalizadas. Alguns exemplos que utilizam este serviço são o Microsoft Exchange Server 2007 e o Microsoft Office SharePoint Server 2007.

O ficheiro da aplicação do serviço de pré-certificação, Precertification.asmx, encontra-se no directório virtual Certification que está no IIS.

Para mais informações sobre a programação de aplicações personalizadas, consulte a Documentação da Tecnologia dos Serviços de Gestão de Direitos na MSDN Library [http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=32972).

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
