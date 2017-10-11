---
TOCTitle: Adicionar Servidores para Suportar a Certificação e o Licenciamento
Title: Adicionar Servidores para Suportar a Certificação e o Licenciamento
ms:assetid: '089ceb62-2a96-444f-ab42-1d5deaabd0c3'
ms:contentKeyID: 18123933
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720189(v=WS.10)'
---

Adicionar Servidores para Suportar a Certificação e o Licenciamento
===================================================================

Após a instalação e o aprovisionamento do primeiro servidor para estabelecimento da instalação de raiz para o RMS, pode configurar servidores adicionais para fornecer suporte expandido aos serviços de certificação e licenciamento, tais como:

-   Pode adicionar um servidor como membro de um cluster de certificações de raiz para fornecer suporte adicional de certificação e de licenciamento. O servidor adicionado a este cluster utiliza a mesma configuração e as mesmas bases de dados do servidor de certificações de raiz.
-   Pode configurar um servidor de licenciamento individual autónomo ou como membro de um cluster de servidores de licenciamento. É pré-inscrito no cluster de certificações de raiz e recebe o certificado de licenciador de servidores (SLC) através dos serviços de certificação do servidor de certificações de raiz. Os pedidos de cliente para serviços de certificação efectuados ao servidor de licenciamento são reencaminhados para o servidor de certificações. O servidor de licenciamento pode emitir licenças de utilização e de publicação sem submeter o pedido ao servidor de certificações de raiz.

A opção que decidir implementar depende da dimensão da organização e da forma como pretende implementar a redundância, o dimensionamento, o suporte de balanceamento de carga e a segurança. Se pretender implementar mais servidores de RMS para satisfazer um número crescente de pedidos de certificação, licenciamento e publicação, deve implementar servidores de RMS como parte do cluster de certificações de raiz para permitir a configuração da redundância e do balanceamento de carga em todos os servidores. Pode agrupar servidores de certificações em clusters e diminuir a carga de processamentos dos serviços de licenciamento e publicação, pré-inscrevendo os servidores de licenciamento (que também podem ser agrupados em clusters para fins de balanceamento de carga). No entanto, não pode efectuar o balanceamento de carga de um cluster de licenciamento pré-inscrito num cluster de certificações de raiz.

Os tópicos seguintes oferecem orientação para esta tarefa:

-   [Funções, Permissões e Direitos Necessários à Instalação e ao Aprovisionamento](#bkmk_1)
-   [Os Processos de Aprovisionamento para Servidores Adicionais de Certificação e Licenciamento](#bkmk_2)
-   [Configurar Clusters e o Balanceamento de Carga](#bkmk_3)

<span id="BKMK_1"></span>
Funções, Permissões e Direitos Necessários à Instalação e ao Aprovisionamento
-----------------------------------------------------------------------------

Para instalar e aprovisionar servidores adicionais, necessita de ter as mesmas funções, permissões e direitos que utilizou para configurar o servidor inicial. Necessita também de ter permissão no servidor de certificações de raiz para configurar um servidor de licenciamento individual. Esta operação é denominada pré-inscrição. O servidor de certificações de raiz é controlado pela lista de controlo de acesso discricionário (DACL) do ficheiro SubEnrollService.asmx. Os membros do Grupo de Serviços do RMS, incluindo a conta de serviço do RMS especificada durante o aprovisionamento do servidor de certificações de raiz, têm permissão para efectuar a pré-inscrição. Para mais informações, consulte "[Configurar Serviços de Certificação e Licenciamento no Primeiro Servidor](https://technet.microsoft.com/cce29a2f-984f-48ed-9187-0eb68286ec5b) anteriormente nesta secção.

<span id="BKMK_2"></span>
Os Processos de Aprovisionamento para Servidores Adicionais de Certificação e Licenciamento
-------------------------------------------------------------------------------------------

Para adicionar servidores a clusters de certificação e de licenciamento é necessário que o servidor efectue o processo de aprovisionamento. O processo de aprovisionamento varia consoante o tipo de servidor a aprovisionar.

-   Se estiver a aprovisionar um servidor de licenciamento individual, especifique uma base de dados de configuração, uma conta de serviço do RMS, o URL do cluster e as informações de protecção de chave privada tal como foram indicados para o servidor de certificações de raiz. No entanto, não especifique uma política de revogação de certificados de licenciadores de servidores, uma vez que essa política é controlada pelo servidor de certificações de raiz.
-   Se estiver a aprovisionar um servidor enquanto membro de um cluster, as únicas informações que tem de especificar durante o aprovisionamento são a conta de serviço do RMS, a base de dados de configuração e a palavra-passe da protecção de chave privada (ou utilize o CSP e a chave privada especificados para o cluster existente). Todos os servidores que fazem parte de um cluster partilham o mesmo certificado de licenciador de servidores e o mesmo par de chaves de servidor.

| ![](images/Cc720189.Important(WS.10).gif)Importante                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Só inicie a instalação do RMS noutros servidores depois de concluir a configuração do RMS no primeiro servidor, incluindo a instalação e o aprovisionamento desse servidor. |

Depois de instalar e aprovisionar um servidor adicional, este é configurado automaticamente como membro do cluster. No entanto, se implementou o balanceamento de carga, tem de configurar o software de balanceamento de carga para funcionar com o novo servidor.

<span id="BKMK_3"></span>
Configurar Clusters e o Balanceamento de Carga
----------------------------------------------

O RMS foi concebido para suportar o agrupamento dos servidores em clusters. A criação de clusters de servidores do RMS aumenta a escalabilidade, a fiabilidade e o balanceamento de carga da implementação do RMS.

**Criar Clusters**

Para configurar um cluster, comece com um servidor de certificações de raiz ou um servidor de licenciamento. Para o segundo servidor e subsequentes pertencentes a cada cluster, instale o RMS no novo servidor, vá para a página **Administração Global** e, em seguida, clique em **Adicionar este servidor a um cluster** para aprovisionar os recursos necessários e associar o servidor ao cluster de certificações de raiz ou ao cluster de licenciamento.

Especifique o nome da base de dados do cluster que pretende associar.

**Clusters de Balanceamento de Carga**

O RMS não implementa automaticamente o balanceamento de carga. Pode utilizar o balanceamento de carga de hardware ou software, incluindo o Balanceamento de Carga em Rede, para balancear a carga nos servidores do RMS.

Os tópicos seguintes fornecem informações mais detalhadas sobre este assunto:

-   Para mais informações sobre as diferenças entre serviços de certificação e de licenciamento, consulte "Descrição Geral do Sistema do RMS" na "Referência Técnica do RMS" nesta recolha de documentação.
-   Para mais informações sobre como mapear implementações de servidor consoante os requisitos de desempenho e disponibilidade da organização, consulte "Fornecer Redundância e Balanceamento de Carga" em "Planear uma Implementação do RMS" nesta recolha de documentação.
-   Para mais informações sobre como determinar o número de servidores necessários para suportar a implementação do RMS na organização, consulte "Avaliar os Requisitos de Dimensionamento" em "Planear uma Implementação do RMS" nesta recolha de documentação.
-   Para mais informações sobre como implementar a segurança de TI na implementação do RMS, consulte "[Proteger a Implementação do RMS](https://technet.microsoft.com/6de8b636-a824-4844-aefc-f26347abfc14)" posteriormente nesta secção.
-   Para mais informações sobre como instalar o RMS, consulte "Para Instalar o RMS com o Service Pack 1" em "Utilizar um Servidor do RMS" nesta recolha de documentação.
    Também pode instalar o RMS a partir de uma linha de comandos. Para mais informações, consulte "Instalação do RMS a partir da Linha de Comandos" em "Utilizar um Servidor do RMS" nesta recolha de documentação.
-   Para mais informações sobre como aprovisionar um servidor de licenciamento, consulte "Para Aprovisionar um Servidor de Licenciamentos" em "Utilizar um Servidor do RMS" nesta recolha de documentação.
-   Para mais informações sobre como aprovisionar servidores adicionais num cluster, consulte "Para Adicionar um Servidor a um Cluster" em "Utilizar um Servidor do RMS" nesta recolha de documentação.
