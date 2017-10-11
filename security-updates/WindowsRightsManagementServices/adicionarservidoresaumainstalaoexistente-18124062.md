---
TOCTitle: Adicionar Servidores a uma Instalação Existente
Title: Adicionar Servidores a uma Instalação Existente
ms:assetid: '7f3598ff-cd19-4daa-aa65-877f7f95a8ec'
ms:contentKeyID: 18124062
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747648(v=WS.10)'
---

Adicionar Servidores a uma Instalação Existente
===============================================

Pode adicionar à instalação do RMS os servidores necessários para satisfazer o aumento da procura ou substituir os servidores que é necessário retirar. Cada instalação do RMS tem de incluir, pelo menos, um servidor de certificação de raiz e, opcionalmente, incluir servidores de certificações de raiz adicionais num cluster. Cada instalação do RMS poderá também incluir servidores de licenciamentos autónomos ou em cluster.

Pode adicionar servidores a uma instalação do RMS através de um dos seguintes métodos:

-   Adicionar um ou mais servidores do RMS a um cluster de certificações de raiz.
-   Adicionar um novo servidor de licenciamentos autónomo.
-   Adicionar um ou mais servidores do RMS a um cluster de licenciamentos.

**Adicionar Servidores de Certificações de Raiz**

Na maioria dos casos, a adição de um ou mais servidores do RMS a um cluster de certificações de raiz é a melhor forma de aumentar a disponibilidade e a redundância da implementação. Um cluster de certificações de raiz é constituído por um ou mais servidores de certificações de raiz. Ao contrário do que se passa com os servidores de licenciamentos, que proporcionam apenas serviços de licenciamento e publicação, os servidores de certificações de raiz disponibilizam todos os serviços do RMS.

Durante a instalação e o aprovisionamento, pode seleccionar a opção de adicionar um servidor a um cluster. Quando seleccionar esta opção, o novo servidor do RMS é configurado automaticamente como membro do cluster. Para ver instruções detalhadas sobre a instalação e o aprovisionamento de um servidor do RMS para adição ao cluster de certificações de raiz, consulte "[Para Instalar o RMS com o Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d)" e "[Para Adicionar um Servidor a um Cluster](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)" posteriormente nesta secção.

Para além do procedimento de aprovisionamento, caso esteja a criar um cluster pela primeira vez, deverá também configurar o software ou hardware com o balanceamento de carga e o funcionamento em cluster adequados. Caso já tenha implementado um cluster, deverá configurar o software ou hardware de balanceamento de carga para trabalhar com o novo membro do cluster.

**Adicionar Servidores de Licenciamento**

Ao contrário do servidor de certificações de raiz, que oferece todos os serviços do RMS, um servidor de licenciamentos fornece apenas serviços de licenciamento e publicação.

Os servidores de licenciamentos são opcionais e implementados, frequentemente, para resolver requisitos específicos de licenciamento, tais como:

-   Suportar requisitos únicos de gestão de direitos de um departamento. Por exemplo, um grupo dentro da sua organização poderá ter requisitos de segurança para a gestão de direitos que não são iguais aos do resto da organização, e poderá pretender ter o controlo total sobre a implementação do licenciamento no grupo. Uma vez que numa floresta é permitido apenas um servidor de certificações de raiz, a configuração de um servidor de certificações de raiz à parte poderá não ser apropriada. Neste caso, pode configurar um servidor ou um cluster de licenciamento dedicado às necessidades desse grupo. Poderá então configurar separadamente a política de direitos para esse servidor ou cluster de licenciamentos.
-   Para suportar a gestão de direitos de parceiros empresariais como parte de uma extranet que exige, para parceiros empresariais específicos, uma separação e um rastreio de recursos rigorosos. Para mais informações, consulte "[Configurar o URL de uma Extranet](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)" posteriormente nesta secção.
-   Para descarregar as tarefas de licenciamento do servidor de certificações de raiz. Esta opção poderá oferecer vantagens em termos de desempenho a organizações que tenham apenas um servidor de certificações de raiz (em vez de um cluster de certificações de raiz).

Para a maioria dos fins, é recomendável a adição de servidores do RMS ao cluster de certificações de raiz para que possa configurar a redundância e o balanceamento de carga em todos os servidores que fazem parte da implementação. Apesar de os servidores de licenciamentos poderem também ser utilizados para descarregar o processamento de pedidos de licenciamento e de publicação, a sua carga não pode ser balanceada com o cluster de certificações de raiz. A não ser que exista a necessidade concreta de implementar servidores de licenciamento separados, recomenda-se balancear a carga por todos os servidores do RMS, tornando-os membros do cluster de certificações de raiz.

Para ver instruções detalhadas para a instalação e o aprovisionamento de um servidor de licenciamentos RMS, consulte "[Para Instalar o RMS com o Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d)" e "[Para Aprovisionar um Servidor de Licenciamento](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)" posteriormente nesta secção.
