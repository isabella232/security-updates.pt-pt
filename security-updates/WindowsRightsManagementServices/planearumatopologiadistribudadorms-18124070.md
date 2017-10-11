---
TOCTitle: Planear uma Topologia Distribuída do RMS
Title: Planear uma Topologia Distribuída do RMS
ms:assetid: '8773a1e0-6ac3-41f5-9866-5890cef08d04'
ms:contentKeyID: 18124070
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747657(v=WS.10)'
---

Planear uma Topologia Distribuída do RMS
========================================

Em algumas circunstâncias, pode ter de implementar um ou mais servidores de licenciamento que não são membros do cluster de certificações de raiz. Normalmente, isto fornece suporte a departamentos que requerem controlo directo para a emissão de licenças de publicação e utilização, como um departamento de contencioso com requisitos de segurança que necessita de controlo a nível departamental. O cluster de certificações de raiz fornece o serviço de certificação de contas aos servidores de licenciamentos. A combinação de um cluster de certificações de raiz com uma ou mais instalações de servidor de licenciamento denomina-se topologia distribuída.

Não se esqueça de que, à semelhança do servidor de certificações de raiz, os servidores de licenciamento também podem ser implementados num cluster. Também à semelhança do cluster de certificações de raiz, o cluster de licenciamento utiliza um serviço de balanceamento de carga próprio. Cada servidor de licenciamentos ou cluster de licenciamentos utiliza uma instância do SQL Server diferente, para fornecer as bases de dados de configuração e de registo a esse servidor ou cluster em particular.

Embora possa configurar a instalação do RMS para executar apenas os serviços de certificação a partir da instalação de raiz e todo o serviço de licenciamento a partir de um ou mais servidores ou clusters de licenciamento, esta não é um topologia típica. De um modo geral, aumenta-se o número de servidores físicos que se encontram no cluster de certificações de raiz de forma a cumprir os requisitos de desempenho e de redundância, em vez de implementar servidores de licenciamentos separados (excepto se for necessário suporte departamental para o licenciamento). O diagrama seguinte ilustra este tipo de implementação.

![](images/Cc747657.01fa5a85-5711-41aa-932a-124049d34186(WS.10).gif)

A criação de uma topologia distribuída pode aumentar os custos administrativos da organização pois a topologia distribuída é inerentemente mais complexa. Se a organização tiver múltiplos clusters de licenciamento e florestas, pode ser necessário substituir o registo dos computadores clientes do RMS para se assegurar de que os pedidos de licenciamento são efectuados no servidor de RMS correcto. Além disso, podem ocorrer problemas de confiança entre domínios. Isto requer a configuração dos domínios para permitir o consumo de conteúdo protegido pelo RMS.

Pontos de Ligação de Serviço numa Topologia Distribuída
-------------------------------------------------------

Quando aprovisiona um servidor do RMS, o URL de um cluster é adicionado à floresta do Active Directory num ponto de ligação de serviço (SCP). Existe um SCP para o cluster de certificações de raiz e para cada cluster de licenciamento aprovisionado na floresta. O SCP tem de ser registado para o cluster de certificações de raiz antes de aprovisionar um cluster de licenciamento. Quando aprovisiona o cluster de licenciamento, o processo de pré-inscrição utiliza o URL para localizar o cluster de certificações de raiz na rede e para obter um certificado de licenciador de servidores.

Quando implementa um cluster de certificações de raiz em vez de um servidor de certificações de raiz, cada servidor existente no cluster tem de ser capaz de ser endereçado virtualmente através de um URL partilhado.

Existem diversas implementações do endereçamento virtual, como o DNS de round-robin, o serviço Balanceamento de Carga em Rede, soluções de hardware, etc. O endereçamento virtual fornece balanceamento de carga nos servidores e também retira a dependência relativamente a um servidor para licenciamento e publicação.

O RMS utiliza o URL partilhado para o URL de aquisição de licenças e para o valor publicado que os computadores de utilizar final utilizam quando procuram o respectivo cluster do RMS no Active Directory ou no registo. Nenhum computador de utilizador final requer acesso directo a um só servidor que esteja num cluster.
