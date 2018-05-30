---
TOCTitle: 'Expandir a infra-estrutura Básica para Suportar Clusters'
Title: 'Expandir a infra-estrutura Básica para Suportar Clusters'
ms:assetid: '78f0f2f0-a075-409c-9f46-26eb62d1d05b'
ms:contentKeyID: 18124063
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747567(v=WS.10)'
---

Expandir a infra-estrutura Básica para Suportar Clusters
========================================================

Se pretender implementar clusters para grandes implementações, certifique-se de que a infra-estrutura está configurada para suportar requisitos de cluster. Os itens seguintes devem ser incluídos nos planos de implementação.

Registo DNS
-----------

Certifique-se de que todos os registos DNS efectuados para expor o endereço IP virtual na extranet também expõem o endereço na intranet.

Se o registo DNS não for efectuado para a intranet, ocorrerão falhas nos pedidos de licença do cliente local. Se não for possível alterar as definições de DNS, a tabela de anfitriões de cada servidor do cluster pode ser modificada para mapear o URL do cluster para o endereço IP virtual do cluster. O registo DNS tem de ser efectuado antes do aprovisionamento do serviço. Se já aprovisionou o serviço, tem de remover o RMS do servidor e repetir o processo de aprovisionamento.

Balanceamento de Carga
----------------------

Configure o hardware e o software necessários para activar a implementação dos servidores de balanceamento de carga, o serviço Balanceamento de Carga em Rede ou o balanceamento de carga de hardware, conforme apropriado, para distribuir os pedidos no cluster.
