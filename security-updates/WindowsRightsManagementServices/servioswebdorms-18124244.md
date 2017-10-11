---
TOCTitle: Serviços Web do RMS
Title: Serviços Web do RMS
ms:assetid: 'ed8dbb2e-0590-4502-afc4-54f66b96d515'
ms:contentKeyID: 18124244
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747728(v=WS.10)'
---

Serviços Web do RMS
===================

O RMS fornece o componente de servidor de um sistema do RMS. As suas funções nucleares são implementadas como um conjunto de serviços Web Microsoft® ASP.NET que são executados nos Serviços de Informação Internet (IIS) da Microsoft®. Os serviços Web do RMS são expostos através da interface SOAP ou .NET Remoting.

Os serviços Web fornecem:

-   Subinscrição de servidores
-   Certificação de contas de entidades fidedignas
-   Licenciamento de informação protegida por direitos
-   Funções de administração do RMS

A tabela seguinte descreve os serviços Web do RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Serviço</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Subinscrição</td>
<td style="border:1px solid black;">Fornece certificados de servidor licenciador subordinado a servidores em clusters apenas de licenciamento. Estes certificados permitem ao cluster apenas de licenciamento emitir licenças de publicação e utilização.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certificação de contas</td>
<td style="border:1px solid black;">Fornece aos utilizadores certificados de contas de direitos. Estes certificados são necessários para que os utilizadores obtenham licenças de publicação e utilização para criar e consumir conteúdo protegido por direitos.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Proxy de activação</td>
<td style="border:1px solid black;">Este serviço é retido para compatibilidade com o cliente do RMS versão 1. Transmite os pedidos de activação da máquina para o Serviço de Activação da Microsoft e devolve cofres e certificados de máquinas RMS a clientes do RMS versão 1. Este serviço não é utilizado por clientes do RMS com Service Pack 1 (SP1) ou posterior.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Publicação</td>
<td style="border:1px solid black;">Emite licenças de publicação, que permitem aos autores criar e distribuir conteúdo protegido por direitos. Emite também certificados de cliente licenciador, que permitem aos utilizadores publicar conteúdo protegido por direitos sem estarem ligados à rede interna que aloja o RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licenciamento</td>
<td style="border:1px solid black;">Emite licenças de utilização, que permitem aos utilizadores consumir conteúdos protegidos por direitos.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Administração</td>
<td style="border:1px solid black;">Permite ao administrador gerir RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">Permite aos serviços Web comunicar entre si e com outros componentes do sistema do RMS expondo o .NET Remoting.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Desactivação</td>
<td style="border:1px solid black;">Transforma conteúdo anteriormente protegido por direitos em conteúdo desprotegido e devolve-o ao cliente. Este serviço é instalado pelo programa de configuração do RMS, mas o serviço não dispõe de uma raiz virtual correspondente no IIS até que seja activado pelo administrador. A activação deste serviço desactiva todos os outros serviços.</td>
</tr>
</tbody>
</table>
  
Além dos serviços Web, o RMS instala um serviço de escuta de registo. Cada serviço Web envia dados registados para a fila de mensagens de registo. O serviço de escuta de registo transfere os dados registados da fila de mensagens para a base de dados de registo.
  
Estas aplicações de serviços Web estão localizadas em directórios virtuais do IIS. Estes directórios virtuais estão instalados em cada servidor do RMS, no Web site seleccionado durante o aprovisionamento.
  
A autenticação e o acesso são configurados em separado para cada directório virtual. Além disso, o acesso é configurado em separado para cada serviço Web. Para obter informações sobre as definições de segurança em directórios virtuais e ficheiros de serviços Web, consulte a secção sobre [Suporte dos Serviços de Informação Internet para o RMS](https://technet.microsoft.com/bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c) posteriormente nesta secção.
  
Para mais informações sobre cada serviço Web, consulte a secção sobre [Componentes de Software do RMS](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca) posteriormente nesta secção.
