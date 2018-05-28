---
TOCTitle: Listas de Revogações do RMS
Title: Listas de Revogações do RMS
ms:assetid: '688d4dfa-c928-4b2f-8116-2f9e87d2b6f7'
ms:contentKeyID: 18124012
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720287(v=WS.10)'
---

Listas de Revogações do RMS
===========================

As listas de revogações especificam o conteúdo, as aplicações, os utilizadores ou outros principais que tenham sido revogados. Uma organização pode incluir uma entidade que esteja numa lista de revogações pelo menos por um dos seguintes motivos:

-   A chave privada é conhecida ou suspeita de ter ficado comprometida.
-   Um proprietário pede a revogação de uma chave que se acredita ter ficado comprometida.
-   Um principal deixou de ser válido (por exemplo, um empregado foi despedido).
-   Existe uma falha na imposição da segurança (por exemplo, um certificado que é emitido para um computador cliente pode ter ficado comprometido).
-   É necessária uma recertificação devido a alterações de autorização.
-   As falhas de segurança existentes numa aplicação activada pelo RMS tornam-na inadequada para ser utilizada no consumo de conteúdo confidencial ou de qualquer conteúdo protegido.
-   Uma peça de conteúdo previamente distribuído que já esteja desactualizado ou impróprio para consumo.

A seguinte tabela descreve as entidades que pode especificar numa lista de revogações, juntamente com as informações que são utilizadas para identificar cada uma.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Entidade</th>
<th>Identificador</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Um grupo de licenças ou certificados</td>
<td style="border:1px solid black;">ID do emissor ou chave pública</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Um grupo de manifestos de aplicações</td>
<td style="border:1px solid black;">ID do emissor ou chave pública</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Uma licença ou certificado específico</td>
<td style="border:1px solid black;">ID de licença ou “hash”</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Um determinado manifesto de aplicação</td>
<td style="border:1px solid black;">ID de licença ou “hash”</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Um determinado principal</td>
<td style="border:1px solid black;">ID do principal ou chave pública</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uma determinada peça de conteúdo</td>
<td style="border:1px solid black;">ID de conteúdo</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720287.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Para a revogação e exclusão, todos os hashes são SHA-1 \[NIS94c\], uma revisão do Secure Hash Algorithm (SHA) especificado na Secure Hash Standard (SHS, FIPS 180). O SHA-1 está descrito no padrão ANSI X9.30 (parte 2). Para revogar por manifesto de aplicação, deve extrair a ID do emissor, a chave pública do emissor, a ID de licença ou hash de licença do manifesto de aplicação. No entanto, os manifestos de aplicações estão codificados numa base 64, para que a informação não esteja disponível logo à partida. Com o Rights Management Client SDK, pode ser desenvolvido um programa utilizando os métodos **DRMConstructCertificateChain**, **DRMDeconstructCertificateChain** e **DRMDecode** para descodificar o manifesto de aplicação e obter as informações necessárias. Se deseja evitar uma determinada capacidade da aplicação de consumir o conteúdo protegido do RMS, considere a utilização da exclusão da aplicação para proibir o servidor RMS de atribuir licenças de utilização a essas aplicações. A limitação da exclusão é que esta não consegue evitar que alguém com uma licença de utilização válida desencripte o conteúdo protegido do RMS. Para mais informações sobre a exclusão de aplicação, consulte Excluir Aplicações em "Utilizar um Servidor do RMS" nesta recolha de documentação. |
  
As listas de revogações são ficheiros XrML que especificam os seguintes parâmetros.
  
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
<td style="border:1px solid black;">ISSUEDTIME</td>
<td style="border:1px solid black;">A hora do sistema quando o ficheiro XrML foi criado. Utilizado pela condição REFRESH existente numa licença de utilização para determinar a idade da lista de revogações.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ISSUER</td>
<td style="border:1px solid black;">O nome, o ID e o endereço do emissor da lista de revogações.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">A chave pública do emissor da lista de revogações.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">REVOCATIONLIST</td>
<td style="border:1px solid black;">O nome, o tipo e o ID de cada entidade revogada.</td>
</tr>
</tbody>
</table>
