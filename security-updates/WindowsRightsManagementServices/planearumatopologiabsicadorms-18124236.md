---
TOCTitle: Planear uma Topologia Básica do RMS
Title: Planear uma Topologia Básica do RMS
ms:assetid: 'fec3201e-201f-4faf-910e-fa44132af83d'
ms:contentKeyID: 18124236
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747755(v=WS.10)'
---

Planear uma Topologia Básica do RMS
===================================

A topologia básica do RMS é composta por um ou mais servidores físicos que agem como cluster de certificações de raiz. Este cluster é utilizado para certificação, licenciamento e publicação na organização. Em todas as implementações, à excepção das mais pequenas, são normalmente configurados vários servidores físicos como um cluster com um só URL. Este cluster é criado através do aprovisionamento do primeiro servidor para criação do servidor de certificações de raiz e através da adição de servidores ao cluster até obter o número de servidores de certificações de raiz necessários ao suporte da actividade projectada. A figura seguinte ilustra este tipo de topologia.

![](images/Cc747755.a3332719-4d25-4694-a89a-7c31fd97ca3b(WS.10).gif)

Quando se associam servidores a um cluster, eles partilham as mesmas bases de dados de configuração e de registo, que são bases de dados do SQL Server. O SQL Server pode residir no servidor de certificações de raiz ou num servidor diferente.

O balanceamento de carga é configurado em todos os servidores que se encontram no cluster de certificações de raiz. Todos os pedidos de certificados e licenças são transmitidos ao cluster de certificações de raiz através do URL comum especificado durante a configuração do primeiro servidor do cluster.

Se só suportar um pequeno número de clientes, pode configurar o RMS num servidor único com uma base de dados local. O servidor é responsável por todas as certificações de licenciamentos da organização. Esta configuração proporciona um ponto de falha único, por isso recomendamos que sejam efectuadas regularmente cópias de segurança da configuração.
