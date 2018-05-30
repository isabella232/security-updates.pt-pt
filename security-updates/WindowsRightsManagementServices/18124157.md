---
TOCTitle: Identificar os Componentes Principais
Title: Identificar os Componentes Principais
ms:assetid: 'c9ec225b-0e51-42f5-aff6-0aecb62e3b27'
ms:contentKeyID: 18124157
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747751(v=WS.10)'
---

Identificar os Componentes Principais
=====================================

Para estabelecer uma topologia adequada, é importante que compreenda os componentes básicos de uma implementação do RMS e das respectivas funções. A lista que se segue identifica os servidores que irão fazer parte da sua implementação do RMS:

-   Servidores de certificações de raiz. O servidor de certificações de raiz é o primeiro componente de uma implementação do RMS. Os restantes componentes dependem dele. O servidor de certificações de raiz executa todos os serviços do RMS, incluindo o serviço de certificações de contas que fornece os certificados de contas de direitos aos clientes do RMS existentes na organização. Só pode existir um servidor de certificações de raiz em cada floresta do Active Directory. No entanto, pode adicionar múltiplos servidores à instalação para criar um cluster de certificações de raiz que pode ser utilizado para fins de redundância e balanceamento de carga. Todos os servidores do cluster de certificações de raiz utilizam a mesma base de dados de configuração definida durante o aprovisionamento do primeiro servidor de certificação na instalação.
-   Servidores de licenciamentos. Um servidor de licenciamento é opcional e não integra o cluster de certificações de raiz. No entanto, o servidor de licenciamento é pré-inscrito no servidor de certificações de raiz. Um servidor de licenciamento depende do servidor de certificações de raiz para fins de certificação e outros serviços (não fornece serviços de certificação de contas), mas executa serviços de licenciamento para fornecer licenças de publicação e utilização. Para configurar a redundância e o balanceamento de carga, pode adicionar múltiplos servidores à instalação para criar um cluster de licenciamento. Todos os servidores existentes no cluster de licenciamento utilizam a mesma base de dados de configuração definida durante o aprovisionamento do primeiro servidor ou cluster de licenciamento.
-   Servidores com componentes de infra-estrutura. Os servidores adicionais que fazem parte da implementação têm capacidade para providenciar a infra-estrutura necessária, incluindo componentes como o SQL Server 2000 e o Active Directory. O local onde estes componentes são implementados e o número de servidores que são necessários depende dos seus requisitos.

A topologia do RMS que estruturar para a organização deve abranger a implementação de cada um destes componentes.
