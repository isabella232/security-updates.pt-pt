---
TOCTitle: Preparação da Recuperação do Sistema
Title: Preparação da Recuperação do Sistema
ms:assetid: '885c047f-1e3b-4bf5-8248-3a4505759cbb'
ms:contentKeyID: 18124072
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747659(v=WS.10)'
---

Preparação da Recuperação do Sistema
====================================

A falha de qualquer um dos componentes do sistema do RMS, incluindo as ligações da Internet e da intranet utilizadas pelo servidor do RMS, o servidor de certificação do RMS, qualquer um dos servidores de licenciamento pré-inscritos do RMS ou os servidores de bases de dados que alojam as bases de dados de configuração do RMS, podem causar a perda inesperada de serviço. Quando configura um sistema do RMS, é importante considerar o impacto potencial nos sistemas de TI e nos dados confidenciais em caso de uma perda de serviço do RMS e preparar a recuperação do componente o mais eficazmente possível.

A falha dos servidores de bases de dados que alojam as bases de dados de configuração do RMS é, provavelmente, o único componente que pode impedir o acesso contínuo às informações protegidas pelo RMS. Esta secção descreve os factores importantes que devem ser considerados na preparação da recuperação de um sistema do RMS, incluindo:

-   [Ligação à Internet](#bkmk_1)
-   [Ligação à Intranet](#bkmk_2)
-   [Serviços de Certificação e Licenciamento](#bkmk_3)
-   [Servidores de Bases de Dados](#bkmk_4)
-   [Active Directory](#bkmk_5)

<span id="BKMK_1"></span>
Ligação à Internet
------------------

Se estiver a utilizar a inscrição online de servidor, o servidor do RMS necessita de ligação à Internet durante o aprovisionamento para obter um certificado de licenciador de servidores (SLC) e efectuar a renovação anual. Quando a data de renovação anual se aproxima, o servidor de certificação notifica-o para renovar o certificado registando eventos no registo de eventos de Sistema. Os eventos são registados mensalmente antes da data de expiração do SLC (ID de Evento 16), semanalmente antes da data de expiração do SLC (ID de Evento ID 17) e quando o SLC expira (ID de Evento 18). A página Web Administração Global do RMS do Web site Administração do RMS alerta-o também sobre a data de expiração do SLC. Se estiver a utilizar o RMS Management Pack para o Microsoft Operations Manager (MOM), os eventos de expiração accionam um alerta. Se a ligação da Internet não estiver disponível no servidor do RMS, o certificado de licenciador de servidores não pode ser renovado com o botão **Renovar** no Web site Administração do RMS e o processo de inscrição offline tem de ser utilizado para pedir um certificado actualizado.

Como procedimento recomendado, renove o SLC antes da data de expiração para evitar problemas caso a ligação à Internet não esteja disponível quando o certificado expirar. O servidor do RMS não pode fornecer serviços do RMS sem um SLC válido, pelo que os utilizadores não conseguirão publicar informações protegidas pelo RMS nem obter licenças de utilização e certificados de contas de direitos (RACs) necessários à leitura das informações protegidas pelo RMS. Os utilizadores, que tenham anteriormente adquirido licenças de utilização e RACs para conteúdo protegido pelo RMS, podem continuar a aceder às informações até as respectivas licenças de utilização ou RACs expirarem.

<span id="BKMK_2"></span>
Ligação à Intranet
------------------

O RMS é uma tecnologia de cliente-servidor que depende de uma infra-estrutura ligada. Sem uma rede de intranet em funcionamento, os servidores do RMS não podem ligar aos serviços necessários na empresa ou aos utilizadores para fornecerem serviços. Sem ligação à intranet, os utilizadores não podem obter certificados de contas de direitos (RACs), certificados de licenciador de clientes (CLCs) e licenças de utilização a partir dos servidores do RMS.

Como procedimento recomendado, as organizações devem optar por arquitecturas de encaminhamento redundantes e ligações de activação pós-falha a partir de sites remotos para os sites do servidor do RMS.

Depois de um utilizador obter um CLC para o respectivo computador, pode publicar informações protegidas pelo RMS em offline quando não existe acesso a um servidor do RMS. Algumas aplicações de correio electrónico activadas pelo RMS foram configuradas para transferirem automaticamente licenças de utilização para as mensagens de correio electrónico associadas protegidas pelo RMS quando sincronizam uma caixa de correio. Desta forma, o utilizador pode ler mensagens de correio electrónico protegidas pelo RMS mesmo quando as ligações à intranet não existem.

<span id="BKMK_3"></span>
Serviços de Certificação e Licenciamento
----------------------------------------

O sistema do RMS depende de dois directórios virtuais dos Serviços de Informação Internet (IIS) 6.0: os serviços de certificação e licenciamento. Estes serviços permitem aos utilizadores e respectivos computadores inscreverem-se no ambiente do RMS e às aplicações activadas pelo RMS publicarem e acederem a informações protegidas pelo RMS. Se estes serviços ficarem indisponíveis, os utilizadores podem negar o serviço até serem repostos.

Para preparar uma potencial perda de serviço, considere criar clusters de servidor de certificação e de servidor de licenciamento pré-inscrito para que divisão de qualquer nó de um cluster não afecte a disponibilidade do serviço.

Como procedimento recomendado, crie capacidade excedentária nos clusters para que as falhas em qualquer um dos nós não afecte o desempenho geral. Quando instalar o primeiro servidor de certificação e cada servidor de licenciamento pré-inscrito ou o primeiro servidor de licenciamento pré-inscrito num cluster, registe cuidadosamente as opções de configuração e os dados introduzidos durante o aprovisionamento.

<span id="BKMK_4"></span>
Servidores de Bases de Dados
----------------------------

Os componentes mais importantes do sistema do RMS são os servidores de bases de dados que mantêm as bases de dados de configuração. Cada servidor ou cluster de servidores do RMS utiliza bases de dados para armazenar informações de configuração e de registo. As informações de configuração são essenciais para o funcionamento do RMS. Estas bases de dados incluem o certificado de licenciador de servidores, os modelos de política produzidos do RMS e uma lista de utilizadores inscritos no sistema do RMS. Se não for utilizado um módulo de segurança de hardware com o servidor do RMS, contêm também as chaves privada e pública do servidor do RMS. As cópias de segurança das bases de dados do RMS permitem restaurar uma instalação anterior do RMS para um servidor novo e recriar um sistema do RMS. O impacto da perda de uma base de dados varia consoante a base de dados. A lista seguinte descreve o impacto de uma falha de uma base de dados específica:

-   **Base de dados de configuração**. Se esta base de dados ficar indisponível durante a utilização do servidor do RMS, os serviços do RMS podem continuar a funcionar pois o RMS coloca as informações necessárias na cache local. No entanto, se ocorrer um evento que requer que o serviço do RMS interaja com a base de dados de configuração, tal como a inscrição de um utilizador novo, o serviço do RMS detecta um erro e o novo utilizador não é capaz de trabalhar com conteúdo protegido pelo RMS. Se ocorrer uma operação que força o servidor do RMS a rejeitar as informações em cache, tal como reiniciar o serviço IIS ou uma renovação agendada da cache local, o serviço do RMS deixa de funcionar. O servidor do RMS só consegue voltar ao serviço normal depois de a base de dados de configuração ficar disponível.
    Se a base de dados de configuração ficar danificada ou permanentemente indisponível, os servidores do RMS deixam de funcionar.
-   **Base de dados dos serviços de directório**. Contém as informações em cache sobre os nomes de grupos e respectivos detalhes de membros obtidos através do servidor de catálogo global. Não ocorre uma redução visível dos serviços do RMS quando esta tabela fica indisponível durante curtos períodos de tempo. Tem por objectivo principal fornecer redundância e cargas de serviço reduzidas para o servidor de catálogo global.
-   **Base de dados de registo**. Se o registo foi activado no servidor do RMS, é a base de dados que deve ser utilizada para armazenar este registo. Se a base de dados não estiver disponível, as entradas de registo acumulam-se no serviço de Colocação de Mensagens em Fila (também denominado MSMQ) no servidor do RMS e ocupam todo o espaço disponível em disco excepto se o serviço for configurado para o não fazer.

Como procedimento recomendado, crie um cluster com os servidores de bases de dados para fornecer protecção de activação pós-falha e activa em espera. Crie regularmente cópias de segurança das bases de dados dos servidores e clusters do RMS, bem como dos servidores e clusters de licenciamento.

Como procedimento recomendado, utilize o envio do registo de transacções como meio de manter uma base de dados de cópia de segurança actualizada. Embora este procedimento possa requerer hardware adicional, permite às organizações recuperarem rapidamente as bases de dados. A equipa de TI da Microsoft implementou este método para a recuperação da base de dados de configuração do RMS. Para tal, seleccione o nome do SQL virtual durante o aprovisionamento do RMS. O nome do SQL virtual permite-lhe mapear o nome do SQL real utilizando o Sistema de Nomes de Domínio (DNS). Caso o SQL Server original deixe de funcionar, pode comutar facilmente para o SQL Server de cópia de segurança alterando o mapeamento do nome de DNS do servidor original para o servidor de cópia de segurança. Para mais informações sobre a implementação interna desta solução da Microsoft, consulte o caso prático da Microsoft no [Web site da Microsoft](http://go.microsoft.com/fwlink/?linkid=42070) (http://go.microsoft.com/fwlink/?LinkId=42070).

<span id="BKMK_5"></span>
Active Directory
----------------

O RMS depende do Active Directory para dois serviços importantes: autenticação de utilizador e serviço de catálogo global. Se o Active Directory ficar indisponível, a autenticação de utilizador não é possível e os utilizadores e respectivos computadores não conseguirão inscrever-se no sistema do RMS. O pipeline de certificação é necessário para a obtenção de um RAC. Este pipeline requer autenticação. Assim que o utilizador obtém um RAC, esse indivíduo pode obter licenças de utilização sem necessitar de outro tipo de autenticação pois o pipeline de autenticação é anónimo por predefinição.

Como as entidades de empresa podem utilizar membros de grupo no Active Directory para exprimirem quem tem acesso às informações protegidas pelo RMS, a perda do Active Directory proibiria os utilizadores de adquirirem licenças de utilização. Por predefinição, as informações de membros de grupo são colocadas na cache do servidor do RMS durante 15 minutos, pelo que uma perda temporária do serviço de catálogo global pode ser tolerada. Modifique a chave de registo que controla o tempo de validade caso pretenda aumentar ou diminuir o período de tempo entre cada actualização da cache. Para mais informações, consulte "Modificar as Definições da Cache do Active Directory" em "Utilizar um Servidor do RMS" nesta colecção de documentação.
