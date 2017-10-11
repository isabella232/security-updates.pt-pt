---
TOCTitle: Guia de Implementação Rápida
Title: Guia de Implementação Rápida
ms:assetid: 'b8fb69b6-3e0b-4836-8c05-8bd93f522a7c'
ms:contentKeyID: 18124133
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747735(v=WS.10)'
---

Guia de Implementação Rápida
============================

Este guia serve para ajudar o utilizador a configurar rapidamente um servidor do RMS com o Service Pack 1 para que possa avaliá-lo e decidir se pretende efectuar uma implementação em grande escala na organização.

**Passo 1 - Preparação do RMS**

O RMS depende de outros componentes que são instalados e configurados antes de utilizar o serviço. A infra-estrutura satisfará os requisitos básicos do RMS depois de concluir os seguintes passos:

1.  Configure um computador com o Windows Server 2003 e, em seguida, associe o computador a um domínio do Active Directory. (Para pequenas organizações que tenham apenas um servidor, este computador também pode ser o controlador de domínio do Active Directory. No entanto, neste caso, o computador tem de utilizar o Windows Server 2003, Standard Edition; o Windows Server 2003, Enterprise Edition; ou o Windows Server 2003, Datacenter Edition. Não é possível que um computador com o Windows Server 2003, Web Edition, seja um controlador de domínio.)
2.  Configure o servidor para o papel de **Servidor de Aplicações**. Para tal, clique em **Iniciar**, faça duplo clique em **Painel de Controlo** e, em seguida, faça duplo clique em **Adicionar ou Remover Programas**. Em **Adicionar ou Remover programas**, clique em **Adicionar/Remover Componentes do Windows** e, em seguida, verifique se os seguintes serviços estão activados em **Servidor de Aplicações**:
    -   **ASP.NET**
    -   **Serviços de Informação Internet (IIS)**
    -   **Colocação de Mensagens em Fila**

    Aceite as opções predefinidas para cada serviço. Não é necessário efectuar mais configurações.
3.  Configure um servidor de bases de dados utilizando uma das seguintes aplicações de base de dados:
    -   Microsoft® SQL Server 2000 com SP3a. Pode tratar-se de uma instalação local do SQL Server 2000 ou de uma instalação remota que se encontre no mesmo domínio.
    -   Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A. Deverá ser uma instalação local. Pode transferir o MSDE 2000 a partir do [Web site da Microsoft](http://go.microsoft.com/fwlink/?linkid=17799) (http://go.microsoft.com/fwlink/?LinkID=17799).

    Recomenda-se a utilização do Microsoft SQL Server Desktop Engine para suportar as bases de dados do RMS apenas em ambientes de teste pois o Microsoft SQL Server Desktop Engine não inclui as ferramentas necessárias para o funcionamento e suporte integrais de uma base de dados empresarial. Adicionalmente, como o MSDE não suporta acesso remoto à rede, tem de instalá-lo no mesmo servidor que o RMS e não pode adicionar outros servidores do RMS ao cluster do RMS. Os termos de utilização do Microsoft SQL Server Desktop Engine especificam que não é possível utilizar ferramentas do cliente SQL Server para manipular uma base de dados do Microsoft SQL Server Desktop Engine. Esta restrição impossibilita a execução de cópias de segurança e o restauro da base de dados de configuração do RMS, a visualização das informações de registo ou a modificação directa de dados armazenados na base de dados de configuração.
4.  Especifique um nome pelo qual este serviço deve ser identificado quando os utilizadores tentam estabelecer ligação na intranet (por exemplo, http://certification.contoso.com). Configure o Sistema de Nomes de Domínio (DNS) para resolver o URL para o endereço de IP do computador do RMS. Deve utilizar um nome de domínio DNS totalmente qualificado para o URL do cluster para se certificar de que os clientes de outras zonas DNS conseguem resolver o endereço IP do servidor ou servidores do RMS.
5.  Crie uma conta de administrador para ser utilizada com o RMS.
6.  Está pronto para instalar o RMS SP1. Para mais instruções sobre este passo, consulte "Para instalar o RMS com o Service Pack 1" em "Utilizar um Servidor do RMS" nesta colecção de documentação.

**Funcionalidades Opcionais Utilizadas Frequentemente**

As funcionalidades indicadas a seguir são opcionais. Se optar por utilizá-las, certifique-se de que implementou todos os preparativos necessários antes de iniciar o processo de instalação e aprovisionamento do RMS:

-   Pode configurar o RMS para utilizar um módulo de segurança por hardware (HSM) para guardar chaves privadas. Se pretender utilizar um módulo de segurança por hardware, certifique-se de que os controladores estão correctamente configurados e de que o mundo de segurança está definido.
-   Pode transferir automaticamente um certificado de licenciador de servidores durante o processo de aprovisionamento se o computador do RMS estiver apto a comunicar com a Internet. Se a organização utilizar um servidor proxy para ligar à Internet, verifique as definições de proxy do Internet Explorer, incluindo quaisquer requisitos de autenticação, e guarde-as para utilização posterior.
-   Se pretender utilizar o RMS num controlador de domínio e planear utilizar uma conta de utilizador para executar os serviços do RMS, certifique-se de que a Política de Segurança do Controlador de Domínio se encontra configurada para conceder permissão à conta de utilizador para iniciar sessão localmente. Para mais informações sobre como configurar a Política de Segurança do Controlador de Domínio, consulte o Centro de Ajuda e Suporte do Windows Server 2003.

**Passo 2 - Aprovisionar o Primeiro Servidor do RMS**

O aprovisionamento é o processo de configuração de um Web site com o RMS para que os utilizadores possam começar a utilizar o serviço. Utilize os seguintes passos para aprovisionar o servidor de certificações de raiz da organização:

1.  Inicie sessão no computador como utilizador de domínio com privilégios de administrador local. Se está a instalar o RMS num controlador de domínio, inicie sessão como administrador de domínio.
2.  Clique em **Iniciar**, aponte para **Todos os Programas**, aponte para **Windows RMS** e, em seguida, clique em **Administração do Windows RMS** para abrir a página **Administração Global**. Esta página apresenta os Web sites disponíveis neste servidor.
3.  Clique no Web site que pretende aprovisionar com o RMS e, em seguida, clique em **Aprovisionar o RMS neste Web site**. Quando a página é aberta, indica **Aprovisionar o Servidor de Certificações de Raiz do RMS** na parte superior.
4.  Preencha a página com as informações da organização.
    -   Na caixa **URL do cluster**, escreva o nome do serviço (por exemplo, certification.contoso.com) que foi configurado no passo 4 do procedimento anterior. Se pretender utilizar o SSL com a instalação, clique no protocolo HTTPS na lista de protocolos. Quando o fizer, o SSL fica activado. No entanto, esta selecção não requer que o SSL seja utilizado nos serviços Web do RMS. Terá de efectuar essa configuração separadamente através do IIS.
    -   Se o servidor estiver ligado à Internet através de um servidor proxy, na área **Definições de Proxy do RMS** preencha a secção com as informações registadas no Internet Explorer como descrito na secção das funcionalidades opcionais do procedimento anterior.
    -   Na área **Ligação à Internet do Servidor**, seleccione **Online** se pretender que o servidor se ligue ao Serviço de Inscrição da Microsoft através da Internet e obtenha um certificado de licenciador de servidores automaticamente durante o processo de aprovisionamento. Seleccione **Offline** se pretender que o servidor se ligue manualmente ao Serviço de Inscrição da Microsoft e transfira o certificado de licenciador de servidores e, em seguida, importe-o após o aprovisionamento do RMS.
5.  Clique em **Submeter**.
    Em aproximadamente 60 a 90 segundos, o aprovisionamento é concluído com êxito, permitindo o regresso à página **Administração Global**, onde pode administrar o servidor do RMS que acabou de aprovisionar.
6.  Na página **Administração Global**, seleccione **Administrar o RMS neste Web site** para abrir a home page **Administração** do servidor do RMS.
    Se seleccionou Offline para Ligação à Internet do Servidor no passo 4, efectue o procedimento "Para Inscrever Manualmente um Servidor de Certificações de Raiz" antes de continuar.
7.  Na home page Administração, clique na ligação **Ponte de Ligação do Serviço do RMS**.

| ![](images/Cc747735.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                  |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| O passo seguinte deste procedimento consiste no registo do ponto de acesso do serviço e requer a utilização de uma conta de domínio com privilégios suficientes para criar um objecto contentor sob o contentor Serviços no contentor Configuração da floresta do Active Directory. O grupo de segurança predefinido, **Admins da empresa**, é um exemplo de uma conta com os privilégios necessários. |

1.  Na página **Ponto de ligação do serviço RMS**, clique no botão **Registar URL**. Isto regista o ponto de ligação do serviço do RMS no Active Directory para que as aplicações activadas pelo RMS possam identificar o licenciamento do RMS, o proxy de activação e os serviços de certificação. 

**Passo 3 - Testar o RMS**

Antes de poder utilizar totalmente o RMS, tem de instalar o cliente dos Serviços de Gestão de Direitos do Microsoft Windows e uma aplicação activada pelo RMS nos computadores clientes. Os utilizadores deverão ser membros do domínio do Active Directory e os computadores cliente deverão ser associados ao domínio. Além disso, os utilizadores do domínio devem todos ter endereços de correio electrónico definidos no Active Directory. Para testar o RMS:

1.  Inicie sessão no computador cliente como utilizador de domínio válido.
2.  Instale o cliente do RMS para o Service Pack 1.
3.  Instale uma aplicação activada pelo RMS.
4.  Crie um ficheiro protegido pelo RMS, conceda direitos só de leitura para esse ficheiro a todos os utilizadores e, em seguida, guarde o ficheiro numa pasta partilhada à qual os utilizadores tenham acesso total.
5.  Inicie sessão no computador como utilizador diferente. Abra o ficheiro e tente efectuar alterações. Se o RMS estiver correctamente instalado, não consegue alterar o ficheiro.
