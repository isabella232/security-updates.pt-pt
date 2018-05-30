---
TOCTitle: Tabelas de Bases de Dados de Registo do RMS
Title: Tabelas de Bases de Dados de Registo do RMS
ms:assetid: '7ab2104c-b12d-4807-8a4b-bcabb145ff9b'
ms:contentKeyID: 18124065
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747569(v=WS.10)'
---

Tabelas de Bases de Dados de Registo do RMS
===========================================

Esta secção descreve as tabelas da base de dados de registo do RMS.

DRMS\_Log\_Master
-----------------

A tabela seguinte mostra a entrada relativa a cada registo.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Tipo de Dados</th>
<th>NULLs</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Não NULL</td>
<td style="border:1px solid black;">ID exclusiva para este registo</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_HostMachineName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Servidor que gerou este registo</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_HostMachineRequestId</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">ID do pedido</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_RequestTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Data e hora do pedido</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestPath</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Caminho do URL do pedido</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Tipo de pedido</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestUserAddress</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Endereço IP do cliente</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestUserAgent</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Cabeçalho do agente do utilizador do cliente</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Estado de autenticação do pedido</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_SecureConnectionState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Protecção SSL do pedido</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedId</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">ID do utilizador autenticado</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ReceivedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">XrML recebido do cliente no pedido</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_IssuedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Licença XrML emitida no pedido</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Metadata</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Metadados</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_SuccessOrFailure</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Êxito ou falha do pedido</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ErrorInformation</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Dados do erro</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_LogCreateTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Tempo de criação do registo</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
A seguinte tabela mostra dados adicionais para um registo. Geralmente, os dados XrML são registados nesta tabela.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Tipo de Dados</th>
<th>NULLs</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogDetailID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1)</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Não NULL (FK)</td>
<td style="border:1px solid black;">ID do registo principal</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_Name</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Nome da propriedade</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Value</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Valor da propriedade</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
A tabela seguinte mostra os campos que o serviço de escuta regista.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Tipo de Dados</th>
<th>NULLs</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Não NULL</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_FieldName</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Nome do campo</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_FieldDescription</td>
<td style="border:1px solid black;">nvarchar(1024)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Descrição do campo</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_IsIncluded</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Indica se o campo está registado</td>
</tr>
</tbody>
</table>
