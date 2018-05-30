---
TOCTitle: Gerir Certificados de Licenciador de Servidores
Title: Gerir Certificados de Licenciador de Servidores
ms:assetid: '549979ad-13ee-4abc-8281-3e002a5a9561'
ms:contentKeyID: 18123989
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720272(v=WS.10)'
---

Gerir Certificados de Licenciador de Servidores
===============================================

Os certificados de licenciador de servidores expiram após um período de tempo especificado, normalmente ao fim de um ano. Para renovar um certificado de licenciador de servidores, é necessário iniciar sessão como administrador local. Quando renovar o certificado de licenciador de servidores para o cluster de certificações de raiz, o RMS envia um pedido de renovação desse certificado para o Serviço de Inscrição da Microsoft. Quando renovar o certificado para um servidor de licenciamentos, o RMS envia um pedido de renovação para o servidor de verificações de raiz que emitiu o certificado que expirou.

Convém controlar os seguintes três eventos enviados pelo RMS para o registo de eventos do sistema. Estes eventos informam os utilizadores de que o certificado de licenciador de servidores está próximo da data de renovação ou expirou. Na tabela seguinte são apresentadas as IDs dos eventos e os respectivos nomes.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>ID do evento</th>
<th>Nome do Evento</th>
<th>Tipo de Evento</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">16</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneMonthEvent</td>
<td style="border:1px solid black;">Aviso. O serviço continua a funcionar normalmente</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneWeekEvent</td>
<td style="border:1px solid black;">Aviso. O serviço continua a funcionar normalmente</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">18</td>
<td style="border:1px solid black;">LicensorCertExpiredEvent</td>
<td style="border:1px solid black;">Erro: O serviço é desactivado.</td>
</tr>
</tbody>
</table>
