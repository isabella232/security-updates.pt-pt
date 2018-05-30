---
TOCTitle: Serviço de Proxy de Activação do RMS
Title: Serviço de Proxy de Activação do RMS
ms:assetid: '6b9d33ef-466b-405b-a768-54e5615d6770'
ms:contentKeyID: 18124040
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747608(v=WS.10)'
---

Serviço de Proxy de Activação do RMS
====================================

Todos os pedidos de activação de computador do RMS versão 1.0 são processados pelo serviço de proxy de activação executado apenas no cluster de raiz do RMS. Tem de activar um computador cliente para o poder utilizar com o RMS para publicar ou consumir conteúdo protegido. A partir do RMS com Service Pack 1, o cliente é de "activação automática" e não necessita de utilizar o servidor proxy de activação nem o Serviço de Activação da Microsoft para gerar um cofre e o certificado de computador.

O serviço de proxy de activação reencaminha os pedidos de activação de computador dos clientes do RMS versão 1.0 para o Serviço de Activação da Microsoft. Este serviço devolve um cofre personalizado e um certificado de computador RMS correspondente que são exclusivos do utilizador e do computador. Em seguida, o serviço de proxy de activação reencaminha estes itens para o cliente que efectuou o pedido.

O ficheiro da aplicação do serviço proxy de activação, Activation.asmx, encontra-se no directório virtual Certification que está no IIS. A lista de controlo de acessos predefinida neste serviço é apresentada na tabela seguinte:

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
<td style="border:1px solid black;">Convidados</td>
<td style="border:1px solid black;">Ler e executar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Grupo de Serviços do RMS</td>
<td style="border:1px solid black;">Ler e executar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SISTEMA</td>
<td style="border:1px solid black;">Controlo total</td>
</tr>
</tbody>
</table>
