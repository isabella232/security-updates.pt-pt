---
TOCTitle: 'Passo 3: Configurar a Ligação de Rede para o WSUS 3.0'
Title: 'Passo 3: Configurar a Ligação de Rede para o WSUS 3.0'
ms:assetid: 'dbc9d9f7-cf52-4539-9f9e-3e823273218a'
ms:contentKeyID: 18142317
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc708602(v=WS.10)'
---

Passo 3: Configurar a Ligação de Rede para o WSUS 3.0
=====================================================

Depois de instalar o WSUS 3.0, o assistente de configuração é iniciado automaticamente. Também pode executá-lo posteriormente através da página **Opções** da consola do WSUS 3.0.

Antes de iniciar o processo de configuração, certifique-se de que sabe as respostas para as seguintes questões:

1. A firewall do servidor está configurada para permitir que os clientes acedam ao servidor?

2. É possível ligar este computador ao servidor a montante (tal como o do Microsoft Update)?

3. Tem o nome do servidor proxy e das credenciais do utilizador para o servidor proxy, se necessário?

Por predefinição, o WSUS está configurado para utilizar o Microsoft Update como localização de obtenção de actualizações. Se tiver um servidor proxy na rede, pode configurar o WSUS para utilizar o servidor proxy. Se houver uma firewall empresarial entre o WSUS e a Internet, poderá ser necessário configurar a firewall de modo a assegurar que o WSUS consegue obter actualizações.

| ![](/security-updates/images/Cc708602.note(WS.10).gif)Nota                                                                                                                  |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Embora tenha de ter ligação à Internet para transferir actualizações do Microsoft Update, o WSUS oferece-lhe a capacidade de importar actualizações para redes não ligadas à Internet. |

**O Passo 3 contém os seguintes procedimentos**:

-   Configurar a firewall.
-   Especificar a forma como este servidor irá obter as actualizações (a partir do Microsoft Update ou de outro servidor WSUS).
-   Configurar as definições do servidor proxy, para que o WSUS possa obter actualizações.

**Para configurar a firewall**
-   Se houver uma firewall empresarial entre o WSUS e a Internet, poderá ser necessário configurar essa firewall de modo a assegurar que o WSUS consegue obter actualizações. Para obter actualizações a partir do Microsoft Update, o servidor WSUS utiliza a porta 80 para o protocolo HTTP e a porta 443 para o protocolo HTTPS. Estas definições não são configuráveis.

-   Se a organização não permitir que a porta 80 ou 443 esteja aberta para todos os endereços, poderá restringir o acesso apenas aos domínios abaixo, de modo a que o WSUS e o serviço Actualizações Automáticas possam comunicar com o Microsoft Update:

    -   http://windowsupdate.microsoft.com
    -   http://\*.windowsupdate.microsoft.com
    -   https://\*.windowsupdate.microsoft.com
    -   http://\*.update.microsoft.com
    -   https://\*.update.microsoft.com
    -   http://\*.windowsupdate.com
    -   http://download.windowsupdate.com
    -   http://download.microsoft.com
    -   http://\*.download.windowsupdate.com
    -   http://wustat.windows.com
    -   http://ntservicepack.microsoft.com

| ![](/security-updates/images/Cc708602.note(WS.10).gif)Nota                                                                                                                                                                                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Estas instruções de configuração da firewall destinam-se a uma firewall empresarial situada entre o WSUS e a Internet. Dado que o WSUS inicia todo o respectivo tráfego de rede, não é necessário configurar a Firewall do Windows no servidor WSUS. |

Embora a ligação entre o Microsoft Update e o WSUS requeira que as portas 80 e 443 estejam abertas, poderá configurar vários servidores WSUS para sincronizarem através de uma porta personalizada.

Os dois procedimentos seguintes assumem que está a utilizar o assistente de configuração. Numa secção posterior deste passo, irá obter informações sobre como iniciar o snap-in Administração WSUS e configurar o servidor através da página **Opções**.

**Para especificar a forma como este servidor irá obter actualizações**
1.  No assistente de configuração, depois de participar no Programa de Melhoramento da Microsoft, clique em **Seguinte** para escolher o servidor a montante.

2.  Se optar por sincronizar a partir do Microsoft Update, concluiu as operações nesta página. Clique em **Seguinte** ou seleccione **Especificar Servidor Proxy** no painel esquerdo.

3.  Se optar por sincronizar a partir de outro servidor, especifique o nome do servidor e a porta em que este servidor comunicará com o servidor a montante.

4.  Para utilizar SSL, marque a caixa de verificação **Utilizar SSL ao sincronizar informações de actualização**. Nesse caso, os servidores irão utilizar a porta 443 para sincronização. (Deve certificar-se de que tanto este servidor como o servidor a montante suportam SSL.)

5.  Se for um servidor de réplica, marque a caixa de verificação **Esta é uma réplica do servidor a montante**.

6.  Nesta altura, concluiu a configuração do servidor a montante. Clique em **Seguinte** ou seleccione **Especificar servidor proxy** no painel esquerdo.

**Para configurar definições de servidor proxy**
1.  Na caixa **Especificar Servidor Proxy** do assistente de configuração, seleccione a caixa de verificação **Utilizar um servidor proxy ao sincronizar** e, em seguida, escreva o nome e número de porta do servidor proxy (por predefinição, a porta 80) nas caixas correspondentes.

2.  Se pretender ligar ao servidor proxy utilizando credenciais de utilizador específicas, seleccione a caixa de verificação **Utilizar credenciais de utilizador para ligar ao servidor proxy** e escreva o nome de utilizador, domínio e palavra-passe do utilizador nas caixas correspondentes. Se pretender activar a autenticação básica para o utilizador que estabelece ligação com o servidor proxy, seleccione a caixa de verificação **Permitir autenticação básica (a palavra-passe é enviada como texto simples)**.

3.  Nesta altura, concluiu a configuração do servidor proxy. Clique em **Seguinte** para ir para página seguinte, onde pode iniciar a configuração do processo de configuração.

Os dois procedimentos seguintes assumem que está a utilizar o snap-in Administração WSUS para a configuração. Estes dois procedimentos mostram como iniciar o snap-in Administração WSUS e configurar o servidor a partir da página **Opções**.

**Para iniciar a consola de Administração do WSUS**
-   Para iniciar a consola Administração WSUS, clique em **Iniciar**, aponte para **Todos os Programas**, aponte para **Ferramentas Administrativas** e, em seguida, clique em **Microsoft Windows Server Update Services 3.0**.

| ![](/security-updates/images/Cc708602.note(WS.10).gif)Nota                                                                                                                                                                                                                                                          |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Para poder utilizar todas as funcionalidades da consola WSUS, tem de ser membro dos grupos de segurança Administradores do WSUS ou Administradores local no servidor no qual o WSUS está instalado. No entanto, os membros do grupo de segurança Informadores WSUS têm apenas acesso só de leitura à consola de administração. |

**Para especificar uma origem de actualização e um servidor proxy**
1.  Na consola WSUS, clique em **Opções** no painel da esquerda, abaixo do nome deste servidor, e clique em **Origem de Actualização e Servidor Proxy** no painel intermédio.

2.  É apresentada uma caixa de diálogo com os separadores **Origem de Actualização** e **Servidor Proxy**.

3.  No separador **Origem de Actualização**, seleccione a localização a partir do qual este servidor irá obter actualizações. Se optar por sincronizar a partir do Microsoft Update (a predefinição), concluiu as operações nesta página do assistente.

4.  Se optar por sincronizar a partir de outro servidor WSUS, necessita de especificar a porta através da qual os servidores irão comunicar (a predefinição é a porta 80). Se escolher uma porta diferente, deverá certificar-se de que ambos os servidores podem utilizar essa porta.

5.  Também pode especificar se pretende utilizar SSL ao sincronizar a partir do servidor WSUS a montante. Nesse caso, os servidores irão utilizar a porta 443 para sincronizar a partir do servidor a montante.

6.  Se este servidor for uma réplica do segundo servidor WSUS, seleccione a caixa de verificação **Esta é uma réplica do servidor a montante**. Neste caso, todas as actualizações têm de ser aprovadas apenas no servidor WSUS.

7.  No separador **Servidor proxy**, seleccione a caixa de verificação **Utilizar um servidor proxy ao sincronizar** e, em seguida, escreva o nome e número de porta do servidor proxy (por predefinição, a porta 80) nas caixas correspondentes.

8.  Se pretender ligar ao servidor proxy utilizando credenciais de utilizador específicas, seleccione a caixa de verificação **Utilizar credenciais de utilizador para ligar ao servidor proxy** e escreva o nome de utilizador, domínio e palavra-passe do utilizador nas caixas correspondentes. Se pretender activar a autenticação básica para o utilizador que estabelece ligação com o servidor proxy, seleccione a caixa de verificação **Permitir autenticação básica (a palavra-passe é enviada como texto simples)**.

9.  Clique em **OK** para guardar estas definições.
