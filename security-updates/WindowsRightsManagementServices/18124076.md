---
TOCTitle: Avaliar os Requisitos de Dimensionamento
Title: Avaliar os Requisitos de Dimensionamento
ms:assetid: '89f0138c-946d-47d7-a286-041d4d9606a8'
ms:contentKeyID: 18124076
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747663(v=WS.10)'
---

Avaliar os Requisitos de Dimensionamento
========================================

Para optar entre a implementação de um ou de múltiplos servidores, determine o número de utilizadores que irão utilizar a implementação do RMS e o número de ficheiros que irão ser protegidos.

Isto permite determinar os requisitos médios de utilização. Planeie os requisitos de utilização de pico. Normalmente, representam o triplo dos requisitos médios.

Considere também os padrões de tolerância a falhas e de disponibilidade de serviços.

Para estabelecer uma medida de benchmark, o RMS foi testado num servidor com processador Pentium 4 duplo de 2,4 GHz e 1 GB de RAM. Nesta configuração, o servidor do RMS emitiu cerca de 50 licenças por segundo.

É possível utilizar os números apresentados a seguir durante a planificação de capacidades, para avaliar os requisitos de utilização de um sistema RMS.

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
<th>Transacção</th>
<th>Ocorrência</th>
<th>Utilização de largura de banda (KB) de cliente-para-servidor</th>
<th>Utilização de largura de banda (KB) de servidor-para-cliente</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Pedido de licença</td>
<td style="border:1px solid black;">Repetido para cada utilizador e para cada peça de conteúdo</td>
<td style="border:1px solid black;">64</td>
<td style="border:1px solid black;">18</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certificação de contas de direitos</td>
<td style="border:1px solid black;">Só tráfego de inicialização do RMS</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">16</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Inscrição de clientes</td>
<td style="border:1px solid black;">Só tráfego de inicialização do RMS</td>
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">16</td>
</tr>
</tbody>
</table>
  
Além disso, o tráfego de consulta do Active Directory pode ter impacto no rendimento da rede. No entanto, não é um factor típico se implementar os servidores do RMS juntamente com os servidores de catálogo global. A excepção seria se uma falha de todos os servidores de catálogo global num site resultasse na falha de outro servidor numa ligação que não suporta a mesma capacidade.
  
A tabela seguinte fornece os dados de base da utilização de largura de banda das transacções do RMS que pode utilizar para avaliar o efeito do tráfego de consultas do Active Directory na rede da organização.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Transacção</th>
<th>Utilização de largura de banda do RMS para o catálogo global (bytes)</th>
<th>Utilização de largura de banda do catálogo global para o RMS (bytes)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Estabelecimento da ligação do RMS (ldap_bind)</td>
<td style="border:1px solid black;">1600</td>
<td style="border:1px solid black;">200</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Avaliação dos membros do grupo do RMS (ldap_search)</td>
<td style="border:1px solid black;">200</td>
<td style="border:1px solid black;">100</td>
</tr>
</tbody>
</table>
  
Quando utilizar estas tabelas de referência, certifique-se de que está a aplicar os números do conteúdo da implementação. Por exemplo, se o utilizador pertencer a 15 grupos, serão necessários 200 bytes para o pedido de procura do RMS e 1500 bytes (100 bytes x 15) para a resposta do catálogo global.
  
O planeamento da capacidade deve basear-se nas cargas previstas de pedidos de licenças para o conteúdo pois estas representam a maioria das operações efectuadas pelo RMS. A velocidade de entrada/saída e o débito do disco rígido não são factores críticos para o RMS porque os pedidos de licença não requerem um grande volume de dados e podem depender totalmente das informações em cache.
  
A utilização da CPU é a variável mais importante quando se determina o rendimento do servidor, por isso é essencial seleccionar os processadores apropriados. Os requisitos de memória dos servidores do RMS aumentam à medida que a carga cresce e ultrapassa o débito máximo do servidor. Quando isto ocorre, os Serviços de Informação Internet (IIS) colocam em fila na memória os pedidos que vão dando entrada, até o servidor os poder processar. Com base no limite da fila configurado no IIS, os pedidos que derem entrada deixam de ser colocados na fila e são rejeitados quando a fila atinge o tamanho máximo especificado.
  
Os requisitos de memória do RMS (conjunto de trabalho) para um padrão de carga devem respeitar totalmente os limites do tamanho da memória física. O tamanho total da memória é mais condicionado pelas necessidades de cache de expansão do grupo do que por qualquer outra coisa. Recomendamos, pelo menos, 1 GB de RAM para cada servidor com o RMS.
  
Cada servidor do RMS é capaz de processar um número definido de pedidos de cliente num período de tempo especificado (cerca de 30 a 50 licenças por segundo). Por este motivo, a adição de servidores reduz a capacidade total de emissão de licenças de um cluster e proporciona também um aumento da fiabilidade. Em resultado disto, o dimensionamento deve ser apropriado não só para cada servidor individualmente, mas também para o total de servidores implementado. Os exemplos de configuração seguintes mostram como pode utilizar estas estimativas para calcular os requisitos de dimensionamento da implementação do RMS.
  
-   Configuração para Utilização Pouco Intensiva  
    Algumas organizações têm requisitos de utilização pouco intensiva para o RMS. Por exemplo, uma organização com cerca de 5.000 utilizadores, dos quais 10 por cento utilizam regularmente o RMS para protegerem conteúdo de correio electrónico, pode calcular que um utilizador médio protege 3 mensagens de correio electrónico por hora. Com base nestes requisitos, os servidores do RMS emitem 1.500 licenças por hora, ou seja, 0,42 licenças por segundo. Obtém assim o requisito de utilização médio; se multiplicar este número por 3 obtém o cálculo da utilização máxima de 1,25 licenças por segundo.  
    Com base neste cálculo, a utilização é bastante ligeira. Por este motivo, um só servidor de RMS seria adequado para esta organização.  
-   Configuração para Utilização Média  
    Muitas organizações têm grupos bastante grandes de grupos de utilizadores com requisitos de utilização moderados. Por exemplo, uma organização com cerca de 40.000 utilizadores, dos quais 50 por cento utilizam regularmente o RMS para protegerem conteúdo, pode calcular que um utilizador médio protege 7 mensagens de correio electrónico e 1 documento ou outro ficheiro por hora. Com base nestes requisitos, os servidores do RMS emitem 160.000 licenças por hora, ou seja, 44,4 licenças por segundo. Obtém assim o requisito de utilização médio; se multiplicar este número por 3 obtém o cálculo da utilização máxima de 133,3 licenças por segundo.  
    Com base neste cálculo, a utilização seria moderadamente elevada, e 6 servidores de RMS seriam apropriados para corresponder às actuais necessidades dos utilizadores, enquanto 10 servidores de RMS corresponderiam às actuais necessidades dos utilizadores, mas com possibilidades de crescimento.  
-   Configuração para Utilização Muito Intensiva  
    As organizações de maiores dimensões têm muitas vezes grupos de utilizadores extremamente grandes com requisitos de utilização intensos. Por exemplo, uma organização com cerca de 150.000 utilizadores, dos quais 70 por cento utilizam regularmente o RMS para protegerem conteúdo, pode calcular que um utilizador médio protege 15 mensagens de correio electrónico e 3 documentos ou outros ficheiros por hora. Com base nestes requisitos, os servidores do RMS emitem 1.890.000 licenças por hora, ou seja, 525 licenças por segundo. Obtém assim o requisito de utilização médio; se multiplicar este número por 3 obtém o cálculo da utilização máxima de 1575 licenças por segundo.  
    Com base neste cálculo, a utilização seria moderadamente elevada, e 32 servidores de RMS seriam apropriados para corresponder às actuais necessidades dos utilizadores, enquanto 51 servidores de RMS corresponderiam às actuais necessidades dos utilizadores, mas com possibilidades de crescimento.
  
Quando os seus cálculos indicarem 30 a 50 licenças entregues por segundo, normalmente isso significa que é necessário outro servidor de RMS.
