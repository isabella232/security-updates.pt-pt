---
TOCTitle: Planear os Requisitos de Cluster para o RMS
Title: Planear os Requisitos de Cluster para o RMS
ms:assetid: 'ec4023eb-4d39-4551-9789-c8a2d973a55b'
ms:contentKeyID: 18124243
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747792(v=WS.10)'
---

Planear os Requisitos de Cluster para o RMS
===========================================

Se estiver a utilizar o RMS numa implementação de cluster, certifique-se de que contempla as condições específicas da organização indicadas a seguir no plano.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Recomendação</th>
<th>Requisito</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Grande número de computadores pessoais utiliza o RMS.</td>
<td style="border:1px solid black;">Pode utilizar o Windows Update, um script ou um método de distribuição de software tal como o Systems Management Server (SMS) ou a Política de Grupo para instalar e activar o software de cliente dos Serviços de Gestão de Direitos do Microsoft Windows.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Grande número de pedidos de clientes.</td>
<td style="border:1px solid black;">Utilize um servidor de balanceamento de carga, como o serviço Balanceamento de Carga em Rede (NLB), ou o balanceamento de carga por hardware para distribuir os pedidos no cluster.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Duas placas de rede utilizam o endereçamento de IP virtual para os pedidos da extranet e da intranet.</td>
<td style="border:1px solid black;">Certifique-se de que todos os registos de DNS efectuados para exporem o endereço de IP virtual à extranet também expõem o endereço à intranet.
Se o registo de DNS não for efectuado para a intranet, ocorrerão falhas nos pedidos de licença de utilização interna. Se não for possível modificar os recursos de DNS, a tabela de anfitriões de cada servidor do cluster pode ser modificada para mapear o URL do cluster para o endereço IP virtual do cluster. O registo de DNS tem de ser efectuado antes do aprovisionamento do RMS. Se já aprovisionou o RMS, desaprovisione-o e, em seguida, repita o processo de aprovisionamento.</td>
</tr>
</tbody>
</table>
