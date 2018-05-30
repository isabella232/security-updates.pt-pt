---
TOCTitle: Certificados de Licenciador de Servidores
Title: Certificados de Licenciador de Servidores
ms:assetid: '0b35fbcd-25a9-4587-898d-9a30fd1d3c5b'
ms:contentKeyID: 18123898
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720184(v=WS.10)'
---

Certificados de Licenciador de Servidores
=========================================

Um certificado de licenciador de servidores concede ao servidor do RMS direitos de emissão de certificados e licenças. Quando o primeiro servidor de certificações de raiz da implementação do RMS é aprovisionado, recebe um certificado de licenciador de servidores do Serviço de Inscrição da Microsoft. Este processo denomina-se inscrição. Este certificado contém a chave pública do servidor de certificações de raiz e está assinado pela chave privada do Serviço de Inscrição. Outros servidores que são adicionados ao cluster de certificações de raiz partilham este certificado.

Durante o aprovisionamento, o primeiro servidor de licenciamento do cluster recebe um certificado de licenciador de servidores do servidor ou cluster de certificações de raiz do RMS num processo denominado pré-inscrição. Este certificado contém a chave pública do servidor de licenciamento e está assinada pela chave privada do servidor ou cluster de certificações de raiz. Outros servidores que são adicionados ao cluster de licenciamento partilham este certificado.

A tabela seguinte apresenta uma lista dos direitos concedidos aos servidores pelos certificados de licenciadores de servidores.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Concede o direito de emitir</th>
<th>Certificado de licenciador de servidores que é emitido para um servidor de certificações de raiz</th>
<th>Certificado de licenciador de servidores que é emitido para um servidor de licenciamentos</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Certificados de conta de direitos</td>
<td style="border:1px solid black;">Sim</td>
<td style="border:1px solid black;">Não</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licenças de publicação</td>
<td style="border:1px solid black;">Sim</td>
<td style="border:1px solid black;">Sim</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licenças de utilização</td>
<td style="border:1px solid black;">Sim</td>
<td style="border:1px solid black;">Sim</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certificados de licenciadores de servidores subordinados</td>
<td style="border:1px solid black;">Sim</td>
<td style="border:1px solid black;">Não</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Certificados de licenciadores de clientes</td>
<td style="border:1px solid black;">Sim</td>
<td style="border:1px solid black;">Sim</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720184.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| O RMS não necessita de servidores ou de clusters de licenciamento separados. No entanto, é possível utilizar servidores e clusters de licenciamento separados para o descarregamento de pedidos do cluster de certificações de raiz. Os administradores também podem configurar servidores de licenciamento para satisfazer as necessidades das organizações internas que necessitam de ter um controlo directo sobre a publicação de conteúdo seguro. Por exemplo, as políticas gerais de uma empresa que estão implementadas nos modelos de política de direitos do servidor ou cluster de certificações de raiz podem não especificar alguns dos direitos exigidos por um determinado departamento. Neste caso, o departamento pode implementar um servidor ou cluster de licenciamentos separado para armazenar os seus modelos de política de direitos e tratar em conformidade os respectivos pedidos de licenciamento. |
