---
TOCTitle: 'FAQ sobre o RMS: Implementação'
Title: 'FAQ sobre o RMS: Implementação'
ms:assetid: '5559ae65-77ae-4e0b-bfd8-3512409ed29b'
ms:contentKeyID: 18123990
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720274(v=WS.10)'
---

FAQ sobre o RMS: Implementação
==============================

Perguntas Mais Frequentes Sobre a Implementação do RMS
------------------------------------------------------

-   [Se os principais de segurança utilizados para o RMS forem membros da lista de endereços global (GAL), existe alguma dependência da versão do Exchange?](#bkmk_20)
-   [Que papel tem o SQL Server no RMS?](#bkmk_21)
-   [O computador do utilizador tem de ser associado ao mesmo domínio do cluster de raiz do RMS para utilizar o RMS?](#bkmk_22)
-   [Se um cliente quiser colocar um servidor do RMS numa rede de perímetro, que portas têm de estar abertas na firewall da Internet e na firewall da intranet para comunicar com o RMS?](#bkmk_23)
-   [De que forma os servidores subordinados num cluster apenas de licenciamento são inscritos e é necessário fazer alguma coisa para os utilizadores terem conhecimento deste cluster?](#bkmk_24)
-   [Qual é a vantagem de utilizar um cluster apenas de licenciamento?](#bkmk_25)
-   [O que é necessário fazer para recuperar completamente uma instalação do RMS?](#bkmk_26)
-   [Depois de desinstalar o cliente do RMS através da funcionalidade Adicionar ou Remover Programas, é necessário remover algum outro ficheiro?](#bkmk_27)
-   [O RMS funciona com o sistema de ficheiros FAT?](#bkmk_28)
-   [Qual é a configuração típica de hardware recomendada para o servidor de base de dados utilizado pelo RMS?](#bkmk_29)
-   [De que forma a utilização do catálogo global do RMS para a expansão de grupos afecta o desempenho do servidor do catálogo geral?](#bkmk_30)
-   [O RMS requer alguma alteração de esquema no Active Directory?](#bkmk_31)
-   [O ponto de ligação do serviço (SCP) será replicado automaticamente entre os diferentes controladores de domínios no domínio em que o cluster do RMS está instalado?](#bkmk_32)
-   [Se os utilizadores não tiverem direitos administrativos nas respectivas máquinas, como é que o cliente do RMS pode ser instalado e configurado?](#bkmk_33)
-   [Qual é a escalabilidade do RMS?](#bkmk_35)
-   [O RMS suporta módulos de segurança do hardware (HSMs) para proteger as chaves do RMS no hardware?](#bkmk_36)

<span id="BKMK_20"></span>
#### Se os principais de segurança utilizados para o RMS forem membros da lista de endereços global (GAL), existe alguma dependência da versão do Exchange?

O RMS depende do Active Directory, mas não do Exchange. No entanto, o Exchange 5.5 mantém o seu próprio directório e não utiliza o Active Directory. Certifique-se de que todos os objectos do grupo e dos utilizadores no Active Directory têm um atributo de correio electrónico válido que inclua o nome do domínio totalmente qualificado. Isto é efectuado automaticamente se estiver a utilizar o Exchange 2000 ou posterior.

<span id="BKMK_21"></span>
#### Que papel tem o SQL Server no RMS?

O RMS utiliza uma base de dados para guardar todos os dados de configuração do serviço, informações sobre os principais no sistema, todos os dados de registo e colocar em cache as pesquisas durante a expansão da lista de distribuição e do Active Directory. O RMS foi completamente testado com o SQL Server 2000 e SQL Server 2005.

<span id="BKMK_22"></span>
#### O computador do utilizador tem de ser associado ao mesmo domínio do servidor do RMS para utilizar o RMS?

O computador do utilizador não tem de ser membro do mesmo domínio do cluster do RMS, mas o computador deverá ser capaz de localizar o cluster do RMS. A forma mais simples de os computadores clientes localizarem o cluster do RMS é a pesquisa do Active Directory através do ponto de ligação do serviço (SCP). No entanto, as definições de registo do cliente podem também ser definidas para localizar o cluster do RMS sem utilizar uma pesquisa do Active Directory. As definições de registo exactas dependem da aplicação activada pelo RMS.

<span id="BKMK_23"></span>
#### Se um cliente quiser colocar o servidor do RMS numa rede de perímetro, que portas têm de estar abertas na firewall da Internet e na firewall da intranet para comunicar com o RMS?

Os utilizadores internos necessitam de aceder aos servidores do RMS que emitem certificados de contas de direitos (RACs) e licenças de utilização. Por predefinição, o servidor do RMS considera o HTTP (TCP porta 80) ou o HTTPS (TCP porta 443), dependendo se o servidor está ou não configurado para utilizar o SSL, pelo que estas portas devem estar abertas na firewall da Internet. É necessário abrir portas adicionais utilizadas por servidores de membros num domínio da firewall da intranet.

<span id="BKMK_24"></span>
#### De que forma os servidores subordinados num cluster apenas de licenciamento são inscritos e é necessário fazer alguma coisa para os utilizadores terem conhecimento deste cluster?

Quando o primeiro servidor do RMS no cluster de raiz for criado numa empresa, recebe um certificado de servidor licenciador do Serviço de Inscrição da Microsoft. Quando for instalado e aprovisionado outro servidor do RMS, pode associá-lo ao cluster de raiz ou inscrevê-lo como um servidor num cluster subordinado apenas de licenciamento. Se o inscrever como um servidor num cluster subordinado apenas de licenciamento, é enviado um pedido de inscrição para o cluster de raiz do RMS. As aplicações activadas pelo RMS especificam em que local uma aplicação de cliente procura o cluster apenas de licenciamento. O Office 2003 é um exemplo de uma aplicação activada pelo RMS que, por predefinição, procura o cluster de raiz. Este comportamento pode ser substituído pelas definições de registo para que a aplicação procure o novo cluster subordinado apenas de licenciamento.

<span id="BKMK_25"></span>
#### Qual é a vantagem de utilizar um cluster subordinado apenas de licenciamento?

Uma vantagem é o isolamento de diferentes departamentos numa organização. Se não for estabelecido um domínio de publicação fidedigno entre o cluster do RMS, o conteúdo só pode ser consumido por utilizadores que tenham acesso a um determinado servidor de licenciamento. Desta forma, um departamento jurídico pode impedir que todos os outros leiam o seu correio electrónico encriptado do RMS. Além disso, pode definir várias opções no cluster apenas de licenciamento, como modelos de direitos, registo, membros do grupo de super utilizadores e políticas de exclusão.

<span id="BKMK_26"></span>
#### O que é necessário fazer para recuperar completamente uma instalação do RMS?

Para reverter uma instalação do RMS, efectue o seguinte procedimento.

**Para reverter uma instalação do RMS**
1.  Remova o ponto de ligação do serviço (SCP) para o cluster do RMS através do Web site de administração do RMS.

2.  Na página de **Administração Global**, clique na opção para **Remover o RMS deste Web site** para desaprovisionar o RMS do servidor. Deverá primeiro desaprovisionar quaisquer servidores subinscritos em clusters apenas de licenciamento e, em seguida, desaprovisionar os servidores de clusters de raiz.

3.  No **Painel de Controlo**, clique em **Adicionar ou Remover Programas** e remova os **Serviços de Gestão de Direitos**.

4.  No servidor da base de dados, remova quaisquer outras bases de dados do RMS restantes.

5.  Remova a conta do serviço do RMS da lista de inícios de sessão autorizados dos servidores de bases de dados e, em seguida, remova a conta do próprio Active Directory.

6.  Se os clientes do RMS estiverem a executar o Windows XP e Windows 2000, remova o cliente do RMS dos computadores clientes.

| ![](images/Cc720274.Important(WS.10).gif)Importante                                                                                                                                                  |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Assim que este procedimento estiver concluído, já não é possível abrir conteúdo protegido por direitos. Desactive primeiro o RMS antes de reverter uma instalação do RMS se o RMS for utilizado para proteger algum dado valioso. |

<span id="BKMK_27"></span>
#### Depois de desinstalar o cliente do RMS através da funcionalidade Adicionar ou Remover Programas, é necessário remover algum outro ficheiro?

Apesar de não ser necessário, pode eliminar o cofre de %systemroot%\\system32.

<span id="BKMK_28"></span>
#### O RMS funciona com o sistema de ficheiros FAT?

Sim, o RMS funciona num computador com FAT, apesar de o sistema de ficheiro NTFS ser recomendado.

<span id="BKMK_29"></span>
#### Qual é a configuração típica de hardware recomendada para o servidor de base de dados utilizado pelo RMS?

A base de dados de registo crescerá rapidamente, especialmente em ambientes em que o RMS é muito utilizado. Se estiver a considerar a utilização do SQL Server para servidor de base de dados, deverá considerar a utilização do SQL Server 2000 Enterprise Edition ou SQL Server 2005 Enterprise Edition no Windows 2000 Advanced Server ou Windows Server 2003, Enterprise Edition, configurado num cluster numa configuração de espera activa. Neste caso, as configurações recomendadas são os discos de registo RAID-1 e os discos de dados RAID-5 e, pelo menos, 512 MB de RAM. O processador mínimo recomendado para esta configuração é um Pentium III a 1,4 GHz. Em servidores de bases de dados dedicados, não são necessários vários processadores.

<span id="BKMK_30"></span>
#### De que forma a utilização do catálogo global do RMS para a expansão de grupos afecta o desempenho do servidor do catálogo geral?

O servidor do RMS colocará em cache quaisquer listas de expansão de grupos, pelo que estas não deverão representar uma grande carga no servidor do catálogo global. As actualizações frequentes aos membros do grupo aumentam a confiança no servidor do catálogo geral, embora o limite de tempo para adquirir novas listas de grupos seja configurável através do registo. A expansão frequente de grupos grandes reduzirá o desempenho. Para mais informações, consulte as informações sobre como Alterar as Definições de Cache do Active Directory, em "RMS: Operações", nesta colecção de documentação.

<span id="BKMK_31"></span>
#### O RMS requer alguma alteração de esquema no Active Directory?

Para que o RMS possa expandir correctamente os membros do grupo especificado na licença de publicação através dos limites da floresta, é necessário existir um objecto de contacto na floresta do Active Directory local que represente o grupo que se encontra na floresta remota. O RMS pode consultar os atributos do objecto de contacto e verificar se esse objecto representa um grupo que está noutra floresta.

Para o RMS o fazer, o Active Directory necessita do atributo de esquema msExchOriginatingForest do Exchange Server 2003 ou posteriores. Este atributo é instalado por predefinição no esquema do Active Directory se tiver um servidor a executar o Exchange Server 2003 na floresta. É necessário ter este atributo na floresta de cada esquema do Active Directory que vai participar no RMS. Se não estiver a utilizar o Exchange Server 2003, pode instalar o esquema separadamente na estrutura do Active Directory utilizando o RMS Administration Toolkit.

<span id="BKMK_32"></span>
#### O ponto de ligação do serviço (SCP) será replicado automaticamente entre os diferentes controladores de domínios no domínio em que o servidor do RMS está instalado?

Depois de aprovisionar o primeiro servidor do RMS numa floresta, deverá ser registado no Active Directory utilizando uma conta de domínio com as permissões suficientes para criar um objecto do contentor sob o contentor de Serviços, no contentor de Configuração, no Active Directory. O grupo de segurança integrada de Administradores de Empresa é um exemplo de uma conta com as permissões requeridas. Isto cria o SCP. Como este está no contentor de Serviços, o Active Directory replica as informações em todos os controladores de domínios da floresta.

<span id="BKMK_33"></span>
#### Se os utilizadores não tiverem direitos administrativos nas respectivas máquinas, como é que o cliente do RMS pode ser instalado e configurado?

O cliente do RMS é um ficheiro do Windows Installer e pode ser distribuído através de uma infra-estrutura de distribuição de software como o Systems Management Server 2003. É também possível distribuir o cliente do RMS utilizando um objecto de política de grupo (GPO) que utilize uma conta de serviço com direitos administrativos. Se o cliente do RMS estiver a executar o Windows Vista, deixa de ser necessária uma instalação do cliente do RMS separada, uma vez que se encontra integrada no sistema operativo.

<span id="BKMK_35"></span>
#### Qual é a escalabilidade do RMS?

O RMS é um serviço Web sem estado e pode ser agrupado em cluster e ter um balanceamento de carga tal como qualquer outro serviço ou Web site. O desempenho do RMS depende sobretudo da disponibilidade do processador, pelo que a adição de processadores pode melhorar o desempenho.

<span id="BKMK_36"></span>
#### O RMS suporta módulos de segurança do hardware (HSMs) para proteger as chaves do RMS no hardware?

Sim, o RMS funciona com o CAPI compatível com os HSMs, como o nCipher HSM.
