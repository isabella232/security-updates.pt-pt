---
TOCTitle: 'Actualizar a Implementação com o RMS Service Pack 2 (SP2)'
Title: 'Actualizar a Implementação com o RMS Service Pack 2 (SP2)'
ms:assetid: '27ee06a1-f467-4a6c-b662-45ddb5f8c13e'
ms:contentKeyID: 18123917
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720225(v=WS.10)'
---

Actualizar a Implementação com o RMS Service Pack 2 (SP2)
=========================================================

Esta secção fornece informações que ajudam o utilizador a instalar os Serviços de Gestão de Direitos do Microsoft® Windows® (RMS, Rights Management Services) com Service Pack 2 (SP2) numa organização com uma implementação do RMS existente. Apenas as organizações que já implementaram o RMS terão necessidade de actualizar a implementação com o RMS com SP2. As organizações que estão a implementar o RMS pela primeira vez podem implementar o RMS com SP2 seguindo as directrizes sobre como Planear uma Implementação do RMS ([http://go.microsoft.com/fwlink/?LinkId=74999](http://go.microsoft.com/fwlink/?linkid=74999)) e Implementar um Sistema do RMS ([http://go.microsoft.com/fwlink/?LinkID=75000](http://go.microsoft.com/fwlink/?linkid=75000)) nesta colecção de documentação.

Pode instalar o RMS com SP2 sem remover a instalação do RMS com SP1 existente. O programa de configuração para o RMS com SP2 detecta se o RMS com SP1 se encontra instalado e adiciona as funcionalidades e definições adicionais consoante necessário.

| ![](/security-updates/images/Cc720225.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                    |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Não é suportado um caminho de actualização do servidor do RMS sem qualquer Service Pack para o RMS com SP2. Se estiver a utilizar um servidor do RMS sem qualquer Service Pack, terá de proceder à actualização para o RMS com SP1 antes de actualizar para o RMS com SP2. O cliente do RMS pode ser actualizado a partir de qualquer versão anterior do cliente do RMS. |

**Nesta secção**

-   [Preparar a actualização do RMS com SP2](#bkmk_preparingforsp2update)
-   [Efectuar a actualização do RMS com SP2](#bkmk_performingsp2update)
-   [Actualizar clusters](#bkmk_updateclusters)
-   [Actualizar clientes do RMS](#bkmk_updateclients)
-   [Interoperabilidade com o RMS versão 1.0](#bkmk_interop)
-   [Remover o RMS com SP2](#bkmk_removingrms)

<span id="bkmk_PreparingForSP2Update"></span>
Preparar a actualização do RMS com SP2
--------------------------------------

A actualização do RMS com SP2 foi concebida de forma a permitir que continue a executar o RMS sem interrupção. No entanto, antes de actualizar o cluster do RMS, recomenda-se que efectue o seguinte:

-   Efectue uma cópia de segurança da base de dados de configuração e da chave privada do RMS. Para mais informações, consulte a secção sobre Cópias de Segurança do Sistema para o RMS ([http://go.microsoft.com/fwlink/?LinkId=75001](http://go.microsoft.com/fwlink/?linkid=75001)) nesta colecção de documentação.
-   Se estiver a utilizar uma chave privada baseada em software, certifique-se de que possui a palavra-passe da chave privada do RMS.
-   Efectue uma cópia de segurança da base de dados de registo caso pretenda reter estatísticas registadas anteriormente.
-   Certifique-se de que dispõe das mais recentes actualizações de alta prioridade e actualizações de segurança para o sistema operativo instalado nos seus clientes e servidores. Para verificar se dispõe de todas as actualizações de alta prioridade e de segurança, clique em **Iniciar**, seguido de **Windows Update** e, em seguida, siga as instruções que surgem no ecrã.

<span id="bkmk_PerformingSP2Update"></span>
Efectuar a actualização do RMS com SP2
--------------------------------------

Quando o assistente de configuração dos Serviços de Gestão de Direitos do Windows com Service Pack 2 detecta a instalação do RMS, a instalação do RMS com SP1 actual é analisada e apenas são adicionados os ficheiros novos ou substituídos aqueles que necessitam de ser alterados para o RMS com SP2. Se já estiver a executar o RMS, não é necessário reaprovisionar ou efectuar qualquer configuração adicional depois de instalar o RMS com SP2 para continuar a executar o RMS.

<span id="bkmk_UpdateClusters"></span>
Actualizar clusters
-------------------

Se instalou o RMS numa configuração de cluster, deve planear a actualização para os clusters a fim de minimizar o impacto da actualização na instalação. Ao determinar a melhor forma de implementar o RMS com SP2 na sua organização, tenha em conta as seguintes recomendações:

-   Como procedimento recomendado, instale o RMS com SP2 numa parte do cluster de cada vez, para que a actualização do cluster possa ser mais previsível e ter menos hipóteses de causar a degradação do serviço durante a actualização.
-   Se tem vários clusters do RMS, deve actualizar os clusters de certificações de raiz em primeiro lugar e, em seguida, actualizar os clusters de licenciamento subinscritos.
-   Se estiver a utilizar a expansão de grupos em florestas, pode actualizar os clusters nas florestas de forma independente sem influenciar a capacidade dos servidores do RMS para expandir a associação a grupos entre florestas.
-   Os servidores do RMS com SP2, RMS com SP1 e RMS versão 1.0 podem coexistir e interagir apenas se se encontrarem em florestas do Active Directory diferentes. Não é recomendada a existência de diferentes versões do servidor do RMS no mesmo cluster.
-   O pacote de configuração do RMS com SP2 pode também ser utilizado para instalar uma nova implementação do RMS com SP2 num servidor; não requer que o RMS com SP1 esteja instalado.

<span id="bkmk_UpdateClients"></span>
Actualizar clientes do RMS
--------------------------

Encontra-se disponível um novo cliente do RMS com SP2 a partir do Windows Update ou do Centro de Transferências da Microsoft. O pacote de configuração de clientes do RMS com SP2 pode também ser usado para instalar uma nova versão do cliente do RMS com SP2 num computador; não requer que o cliente do RMS versão 1.0 esteja instalado. O cliente do RMS com SP2 inclui uma funcionalidade de retro-compatibilidade para permitir a utilização com aplicações activadas pelo RMS que requeiram o RMS versão 1.0.

Para mais informações sobre a actualização e instalação de clientes do RMS, consulte a secção sobre como Distribuir o Cliente do RMS ([http://go.microsoft.com/fwlink/?LinkId=75070](http://go.microsoft.com/fwlink/?linkid=75070)).

<span id="bkmk_InterOp"></span>
Interoperabilidade com o RMS versão 1.0
---------------------------------------

Uma vez que o RMS com SP2 fornece muitos melhoramentos e optimizações de desempenho, deve ser instalado durante o próximo ciclo de actualização. Apesar de os servidores e clientes do RMS que executam o RMS com SP2 serem totalmente interoperáveis com servidores e clientes do RMS que não executam o RMS com SP2, tenha em consideração as seguintes diferenças na forma como funcionam num ambiente misto:

-   Apenas os servidores que executam o RMS com SP1 e posteriores têm capacidade para inscrição offline.
-   Apenas os clientes que executam o RMS com SP1 e posteriores têm capacidade para activação automática.
-   A tabela seguinte menciona as funcionalidades suportadas em ambientes mistos:

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
<th>Versão do Servidor do RMS</th>
<th>Funcionalidades suportadas com clientes da versão 1</th>
<th>Funcionalidades suportadas com clientes do SP2</th>
<th>Funcionalidades suportadas em ambientes de clientes mistos</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1.0</td>
<td style="border:1px solid black;">Todas as funcionalidades anteriores.
Sem inscrição offline do servidor. O servidor tem de efectuar a inscrição através da Internet.
Sem clientes com activação automática.</td>
<td style="border:1px solid black;">Todas as funcionalidades anteriores.
Sem inscrição offline do servidor.
Clientes com activação automática.</td>
<td style="border:1px solid black;">Todas as funcionalidades anteriores.
Os clientes do SP2 têm activação automática.
Os clientes da versão 1 têm de efectuar a activação através da Internet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP2</td>
<td style="border:1px solid black;">Todas as funcionalidades anteriores.
Inscrição offline do servidor.
Sem clientes com activação automática.</td>
<td style="border:1px solid black;">Todas as funcionalidades do SP1.
Inscrição offline do servidor.
Clientes com activação automática.
Cofre para o servidor.
O Microsoft SQL Server™ 2005 é suportado de imediato.</td>
<td style="border:1px solid black;">Todas as funcionalidades anteriores e as funcionalidades do SP2.
Inscrição offline do servidor.
Os clientes do SP2 têm activação automática.
Os clientes da versão 1 têm de efectuar a activação através da Internet.</td>
</tr>
</tbody>
</table>
 

<span id="bkmk_RemovingRMS"></span>
Remover o RMS com SP2
---------------------

Se, após instalar o RMS com SP2, pretender que o servidor do RMS volte à configuração anterior, pode utilizar **Adicionar ou Remover Programas** no **Painel de Controlo** para remover o RMS com SP2.
