---
TOCTitle: Descrição Geral do Sistema do RMS
Title: Descrição Geral do Sistema do RMS
ms:assetid: 'cbd14635-e17e-42b8-9fd8-6fdce42ffe07'
ms:contentKeyID: 18124196
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747671(v=WS.10)'
---

Descrição Geral do Sistema do RMS
=================================

Este tópico fornece informações sobre como os serviços Web do RMS e as tecnologias do cliente do RMS interagem num sistema do RMS.

A tabela seguinte lista os tipos de servidores envolvidos numa implementação do RMS e descreve as respectivas funções. Para mais informações detalhadas sobre a implementação, consulte "Implementar um Sistema do RMS" nesta recolha de documentação.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Servidor ou Cluster</th>
<th>Função</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Certificação de raiz</td>
<td style="border:1px solid black;">Executa os seguintes serviços do RMS:
<ul>
<li><strong>Pré-inscrição</strong>. Pré-inscreve os servidores de licenciamento.<br />
<br />
</li>
<li><strong>Proxy de activação</strong>. Age como um proxy da Internet para os pedidos de cliente de cofres e certificados de computador do RMS.<br />
<br />
</li>
<li><strong>Certificação</strong>. Emite certificados de conta de direitos.<br />
<br />
</li>
<li><strong>Publicação</strong>. Emite licenças de publicação.<br />
<br />
</li>
<li><strong>Licenciamento</strong>. Emite licenças de utilização.<br />
<br />
</li>
</ul>
Cada implementação deve incluir, pelo menos, um servidor ou um cluster de certificações de raiz. Só pode existir um cluster de certificações de raiz por floresta do Active Directory.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licenciamento (opcional)</td>
<td style="border:1px solid black;">Executa os seguintes serviços do RMS:
<ul>
<li><strong>Publicação</strong>. Emite licenças de publicação.<br />
<br />
</li>
<li><strong>Licenciamento</strong>. Emite licenças de utilização.<br />
<br />
</li>
</ul>
Na maior parte das vezes, os servidores de licenciamentos são implementados para suportar departamentos distintos ou para descarregar pedidos de licenciamento do cluster de certificações de raiz. Os servidores de licenciamentos são opcionais.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Servidor de bases de dados, como o SQL Server</td>
<td style="border:1px solid black;"><ul>
<li>Execute as bases de dados de serviços de configuração, registo e directório do RMS.<br />
<br />
</li>
<li>Armazena os certificados de conta de direitos na base de dados de configuração do cluster de certificações de raiz.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Controlador de domínio e catálogo global</td>
<td style="border:1px solid black;"><ul>
<li>Fornece os serviços de autenticação de utilizador e de directórios.<br />
<br />
</li>
<li>Armazena a localização da identificação do serviço do cluster de certificações de raiz.<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

O RMS utiliza os serviços de Inscrição e Activação alojados pela Microsoft para fornece uma raiz comum de fidedignidade ao sistema. Para mais informações, consulte "[Hierarquia de Fidedignidade do RMS](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a)" posteriormente nesta secção.

O diagrama seguinte ilustra os diversos componentes de um sistema do RMS e as respectivas funções no sistema. As setas representam pedidos e respostas a serem trocados entre os diferentes componentes.

![](/security-updates/images/Cc747671.29138741-d45c-459b-8ead-b9bc3f708dd5(WS.10).gif)

Para mais informações sobre cada componente, consulte "[Componentes de Software do RMS](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca)" posteriormente nesta secção.
