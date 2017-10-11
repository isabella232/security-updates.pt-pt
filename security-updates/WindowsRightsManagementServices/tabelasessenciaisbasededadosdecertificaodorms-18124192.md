---
TOCTitle: Tabelas Essenciais à Base de dados de Certificação do RMS
Title: Tabelas Essenciais à Base de dados de Certificação do RMS
ms:assetid: 'd392663a-1a46-42f6-a71d-f0f2c1843566'
ms:contentKeyID: 18124192
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747760(v=WS.10)'
---

Tabelas Essenciais à Base de dados de Certificação do RMS
=========================================================

Este tópico descreve as tabelas de certificação existentes na base de dados de configuração do RMS. As tabelas contêm informações sobre os certificados de conta de direitos emitidos para os utilizadores desta instalação.

UD\_Machines
------------

A tabela seguinte lista as informações sobre as ID do hardware de todos os computadores.

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
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) Não NULL</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PubKeyHash</td>
<td style="border:1px solid black;">binary(20)</td>
<td style="border:1px solid black;">(20) Não NULL</td>
<td style="border:1px solid black;">Hash da ID do hardware</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Data e hora em que a entrada foi adicionada à tabela</td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
A tabela seguinte lista as informações do Microsoft® .NET Passport relativas aos utilizadores.
  
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i64_Puid</td>
<td style="border:1px solid black;">bigint</td>
<td style="border:1px solid black;">(50) NULL</td>
<td style="border:1px solid black;">ID do utilizador do .NET Passport</td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
A tabela seguinte associa os utilizadores certificados às informações dos seus respectivos computadores.
  
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
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Data e hora em que a entrada foi adicionada à tabela</td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
A tabela seguinte lista as informações relativas aos dados dos utilizadores.
  
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) Não NULL</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_KeyData</td>
<td style="border:1px solid black;">varbinary(2000)</td>
<td style="border:1px solid black;">(2000) Não NULL</td>
<td style="border:1px solid black;">Chave pública/privada encriptada do utilizador</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_KeyDataLength</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Tamanho da chave pública/privada desencriptada</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Chave pública do utilizador</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_EncryptionDbId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Índice para o certificado de licenciador utilizado para encriptar o par de chaves pública/privada</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Não especificado</td>
<td style="border:1px solid black;">Não utilizado</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_Expiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Data de expiração da chave do utilizador</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_TemporaryExpiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Data e hora de expiração da utilização temporária da chave</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">f_Modified</td>
<td style="border:1px solid black;">bit</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Não utilizado</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_Quota</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Nível actual da quota relativa ao utilizador</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_WaitDays</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Número de dias a decorrer até que os pedidos de quota adicionais sejam satisfeitos</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_LastConsumption</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Data e hora da última certificação adicional de utilizador</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Data e hora em que a entrada foi adicionada à tabela</td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
A tabela seguinte mostra as ID de todos os utilizadores certificados e autenticados do Windows.
  
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">Índice interno</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Sid</td>
<td style="border:1px solid black;">Sid</td>
<td style="border:1px solid black;">Não NULL</td>
<td style="border:1px solid black;">ID de segurança (SID) do utilizador</td>
</tr>
</tbody>
</table>
