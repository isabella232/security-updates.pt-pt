---
TOCTitle: Retirar Servidores
Title: Retirar Servidores
ms:assetid: '52005e2e-9563-4ba0-906c-3cc76f9c378f'
ms:contentKeyID: 18124017
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747568(v=WS.10)'
---

Retirar Servidores
==================

Em alguns casos, poderá ser necessário retirar um servidor do RMS, devido, por exemplo, às seguintes situações:

-   Problemas com o equipamento ou actualizações, que resultam na substituição de servidores específicos.
-   Diminuição do tráfego de licenciamento e publicação, resultante da desactivação de alguns servidores.
-   Existência de regulamentações que exijam a remoção de servidores de localizações específicas, o que pode implicar a desactivação de um cluster inteiro.
-   Fusão ou venda de divisões ou outras áreas da organização, resultando na transferência de activos.
-   Fusão da totalidade da organização com outra organização que tem igualmente o RMS, tornando ambas as instalações do RMS redundantes.

Antes de retirar um servidor, deverá efectuar uma cópia de segurança de todas as bases de dados do RMS utilizadas pelo servidor, em especial da base de dados de configuração. Para mais informações sobre como efectuar cópias de segurança das bases de dados, consulte "Efectuar Cópias de Segurança e Restaurar o Sistema para o RMS" na secção "Planear uma Implementação do RMS" nesta colecção de documentação. .

Depois de ter feito uma cópia de segurança das bases de dados, pode remover o servidor. Os requisitos da remoção de um servidor do RMS dependem da função do servidor e da tipologia da instalação do RMS:

-   **Remover um servidor de um cluster**. Se o servidor do RMS que pretende retirar está num cluster que tem outros servidores do RMS ainda activos e que são necessários, a remoção de um servidor individual do cluster exige o desaprovisionamento e a desinstalação do RMS do servidor em causa, a remoção do hardware do cluster e o arquivamento das bases de dados.
    | ![](images/Cc747568.note(WS.10).gif)Nota                                                                                                                       |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Apenas os servidores do cluster de certificação de raiz devem ser desaprovisionados antes da desinstalação do RMS. Este procedimento não é necessário para os servidores de licenciamentos. |

-   **Retirar um servidor autónomo**. Se o servidor do RMS que pretende retirar é um servidor autónomo (ou seja, que não faz parte de um cluster multi-servidores), substituindo-o por um novo servidor, execute os seguintes passos: desaprovisione e desinstale o servidor existente do RMS, retire-o da rede e instale e aprovisione imediatamente o RMS no servidor substituto. Configure o novo servidor do RMS para que utilize o mesmo URL e a mesma base de dados de configuração utilizados pelo antigo servidor do RMS. Lembre-se de que os utilizadores não podem consumir o conteúdo publicado pelo servidor retirado até que o servidor que o substituiu seja instalado e aprovisionado.
    | ![](images/Cc747568.Important(WS.10).gif)Importante                                                                                                                                                                                                                     |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Se o servidor do RMS que está a substituir utiliza um módulo de segurança por hardware, deverá transferir o mundo de segurança para o novo servidor antes de aí instalar e aprovisionar o RMS. Para obter mais instruções, consulte a documentação que acompanha o módulo de segurança por hardware. |

-   **Substituir a instalação do RMS por uma outra existente**. Em alguns casos, poderá necessitar de retirar a instalação do RMS e substitui-la por outra instalação existente, como, por exemplo, no caso de uma fusão de empresas em que ambas utilizam o RMS.

Quando desaprovisiona e desinstala um servidor, este é removido da tabela ClusterServer da base de dados de configuração e a base de dados de serviços de directório é apagada do SQL Server. Para mais instruções para o desaprovisionamento e a desinstalação do RMS, consulte "[Para Desaprovisionar o RMS](https://technet.microsoft.com/9fa63daa-5fb9-4afd-8371-b38248619857)" e "[Para Desinstalar o RMS](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)" posteriormente nesta secção.
