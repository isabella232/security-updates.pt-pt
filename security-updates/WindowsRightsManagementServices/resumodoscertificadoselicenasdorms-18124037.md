---
TOCTitle: Resumo dos Certificados e Licenças do RMS
Title: Resumo dos Certificados e Licenças do RMS
ms:assetid: '637ccfca-318e-4346-85b5-0945b058fb9c'
ms:contentKeyID: 18124037
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747595(v=WS.10)'
---

Resumo dos Certificados e Licenças do RMS
=========================================

A tabela seguinte lista os certificados e as licenças utilizados pelo RMS. São analisados detalhadamente nos tópicos restantes desta secção.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Certificado ou licença</th>
<th>Finalidade</th>
<th>Conteúdo</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Certificados de licenciadores de servidores</td>
<td style="border:1px solid black;">Os certificados de licenciadores de servidores que são emitidos para os servidores de licenciamentos concedem o direito de emitir:
<ul>
<li>Licenças de publicação<br />
<br />
</li>
<li>Licenças de utilização<br />
<br />
</li>
<li>Certificados de licenciadores de clientes<br />
<br />
</li>
<li>Modelos de política de direitos<br />
<br />
</li>
</ul>
Os certificados de licenciadores de servidores que são emitidos para o cluster de certificações de raiz concedem, também, o direito de emitir:
<ul>
<li>Certificados de contas de direitos para clientes<br />
<br />
</li>
<li>Certificados de licenciadores de servidores para servidores de licenciamentos<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">O certificado de licenciador de servidores que é emitido para um servidor de licenciamentos contém a chave pública do servidor de licenciamentos.
O certificado de licenciador de servidores que é emitido para o servidor de certificações de raiz contém a chave pública do servidor de certificações de raiz.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certificados de licenciadores de clientes</td>
<td style="border:1px solid black;">Concedem ao utilizador o direito de publicar conteúdo protegido pelo RMS sem estar ligado à rede da empresa.</td>
<td style="border:1px solid black;">Contêm a chave pública do certificado e a chave privada do certificado encriptado pela chave pública do utilizador que pediu o certificado. Contêm, também, a chave pública do servidor que emitiu o certificado.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Certificados de computador do RMS</td>
<td style="border:1px solid black;">Identificam um computador ou dispositivo considerado fidedigno pelo sistema do RMS.</td>
<td style="border:1px solid black;">Contêm a chave pública do computador activado. A chave privada correspondente é contida no cofre do computador.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certificados de conta de direitos</td>
<td style="border:1px solid black;">Identificam um utilizador relativamente a um determinado computador ou dispositivo.</td>
<td style="border:1px solid black;">Contêm a chave pública do utilizador e a correspondente chave privada que está encriptada com a chave pública do computador activado.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licenças de publicação</td>
<td style="border:1px solid black;">Especificam os direitos aplicáveis ao conteúdo protegido pelo RMS.</td>
<td style="border:1px solid black;">Contêm a chave de conteúdo simétrica para desencriptação do conteúdo encriptado com a chave pública do servidor que emitiu a licença.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licenças de utilização</td>
<td style="border:1px solid black;">Especificam os direitos aplicáveis ao conteúdo protegido pelo RMS no contexto de um utilizador autenticado específico.</td>
<td style="border:1px solid black;">Contêm a chave de conteúdo simétrica para desencriptar o conteúdo, o qual está encriptado com a chave pública do utilizador.</td>
</tr>
</tbody>
</table>
