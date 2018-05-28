---
TOCTitle: 'Passo 4: Configurar Actualizações e a Sincronização'
Title: 'Passo 4: Configurar Actualizações e a Sincronização'
ms:assetid: '734cc2ed-98be-4772-a42c-8fd38b39d864'
ms:contentKeyID: 18142194
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc708447(v=WS.10)'
---

Passo 4: Configurar Actualizações e a Sincronização
===================================================

Antes transferir actualizações, será necessário especificar que actualizações pretende transferir. Esta secção descreve como configurar o conjunto de actualizações que pretende transferir.

Os procedimentos neste passo descrevem como:

-   Guardar e transferir informações sobre o servidor a montante e o servidor proxy.
-   Escolher o idioma das actualizações pretendidas.
-   Escolher os produtos para os quais pretende obter actualizações.
-   Escolher as classificações de actualizações pretendidas.
-   Especificar a agenda de sincronização para este servidor.

Os cinco procedimentos seguintes descrevem como configurar as actualizações utilizando o assistente de configuração. Os procedimentos posteriores descrevem como efectuar esta configuração a partir da consola de Administração do WSUS escolhendo opções específicas.

**Guardar e transferir informações sobre o servidor a montante e o servidor proxy**
1.  Deve concluir a configuração do servidor a montante e do servidor proxy no assistente de configuração e deve utilizar a página **Ligar ao Servidor a Montante**.

2.  Clique no botão **Iniciar Ligação**, que irá guardar e carregar as definições, e obtenha informações sobre actualizações disponíveis.

3.  Enquanto a ligação estiver a ser estabelecida, o botão **Parar Ligação** ficará disponível. Se existirem problemas com a ligação, clique em **Parar Ligação**, corrija os problemas e reinicie a ligação.

4.  Depois de a transferência ter sido concluída com êxito, clique em **Seguinte** para ir para a página **Escolher Idiomas** ou seleccione uma página diferente no painel esquerdo.

**Escolher idiomas da actualização**
1.  A página **Escolher Idiomas** permite obter actualizações a partir de todos os idiomas ou de um subconjunto de idiomas. A selecção de um subconjunto de idiomas poupa espaço em disco, mas é importante que escolha todos os idiomas que serão necessários por todos os clientes deste servidor WSUS.

2.  Se optar por obter actualizações para apenas alguns idiomas, seleccione **Transferir actualizações apenas nestes idiomas** e seleccione os idiomas para os quais pretende actualizações. Clique em **Seguinte** para avançar para a página **Escolher Produtos** ou seleccione uma página diferente no painel esquerdo.

**Escolher produtos de actualização**
1.  A página **Escolher Produtos** permite especificar os produtos para os quais pretende actualizações.

2.  Poderá marcar categorias de produto, tal como o Windows ou produtos específicos, tal como o Windows Server 2003. A selecção de uma categoria irá fazer com que todos os produtos subjacentes sejam seleccionados. Clique em **Seguinte** para avançar para a página **Escolher Classificações** ou seleccione uma página diferente no painel esquerdo.

**Escolher classificações de actualização**
1.  A página **Escolher Classificações** permite escolher as classificações de actualizações que pretende obter. Pode escolher todas as classificações ou um subconjunto das mesmas.

2.  Clique em **Seguinte** para avançar para a página **Configurar Agenda de Sincronização** ou seleccione uma página diferente no painel esquerdo.

**Configurar a agenda de sincronização**
1.  Verá a página **Definir Agenda de Sincronização**, que permite escolher entre a execução manual ou automática da sincronização.

2.  Se escolher sincronizar manualmente neste servidor, terá de iniciar o processo de sincronização a partir da consola de Administração do WSUS.

3.  Se escolher sincronizar automaticamente, o servidor WSUS será sincronizado a intervalos especificados. Defina a hora da primeira sincronização e especifique o número de sincronizações por dia que pretende que este servidor efectue. Por exemplo, se especificar a execução de quatro sincronizações por dia, com início às 03:00, as sincronizações terão lugar às 03:00, 09:00, 15:00 e 21:00.

Depois de ter concluído todos os passos de configuração anteriores, seleccione a página **Concluído** no assistente de configuração. Pode iniciar a consola a consola de Administração do WSUS deixando a caixa de verificação **Iniciar o snap-in de Administração do Windows Server Update Services** e pode iniciar a primeira sincronização deixando a caixa de verificação **Iniciar sincronização inicial**.

| ![](/security-updates/images/Cc708447.note(WS.10).gif)Nota                                                                                                  |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Não é possível guardar alterações de configuração efectuadas durante a sincronização do servidor. Aguarde até a sincronização ter terminado de efectuar as alterações. |

![](/security-updates/images/Cc708447.3f774fd1-af87-47d8-8f50-a5d585687d70(WS.10).gif)

Os seguintes procedimentos explicam como efectuar os passos de configuração anteriores através da página **Opções** da consola de Administração do WSUS:

-   Escolher produtos e classificações
-   Idiomas e ficheiros de actualização

**Escolher produtos e classificações**
1.  Inicie a consola de Administração do WSUS: Clique em **Iniciar**, aponte para **Todos os Programas**, aponte para **Ferramentas Administrativas** e, em seguida, clique em **Microsoft Windows Server Update Services**.

2.  Seleccione **Opções** abaixo do servidor WSUS no painel esquerdo.

3.  No painel intermédio, seleccione **Produtos e Classificações**.

4.  Verá uma caixa de diálogo com dois separadores: **Produtos** e **Classificações**.

5.  No separador **Produtos**, seleccione a categoria de produto ou o produto específico para o qual pretende que este servidor obtenha actualizações, ou seleccione **Todos os Produtos**.

6.  No separador **Classificações**, seleccione as classificações de actualizações pretendidas ou seleccione **Todas as Classificações**.

7.  Clique em **OK** para guardar as selecções.

**Idiomas e ficheiros de actualização**
1.  Na página **Opções**, seleccione **Idiomas e Ficheiros de Actualização**.

2.  Verá uma caixa de diálogo com dois separadores: **Ficheiros de Actualização** e **Idiomas de Actualização**.

3.  No separador **Ficheiros de Actualização**, pode optar por armazenar os ficheiros de actualização localmente ou definir que todos os computadores cliente instalem a partir do Microsoft Update. Se optar por armazenar os ficheiros de actualização neste servidor, pode optar por transferir apenas as actualizações aprovadas ou transferir ficheiros de instalação rápida.

4.  No separador **Idiomas de Actualização**, pode optar por obter actualizações para todos os idiomas (a predefinição) ou por obter actualizações para apenas os idiomas especificados. Se este servidor WSUS tiver servidores a jusante, irá obter actualizações apenas nos idiomas especificados pelo servidor a montante.

5.  Clique em **OK** para guardar estas definições.

Depois de configurar a ligação de rede, poderá transferir actualizações através da sincronização do servidor WSUS.

A sincronização implica que o servidor WSUS contacte o Microsoft Update. Após o contacto, o WSUS determina se foram disponibilizadas novas actualizações desde a última sincronização. Dado que se trata da primeira vez que está a sincronizar o servidor WSUS, todas as actualizações estão disponíveis e prontas para aprovação para instalação. A sincronização pode demorar bastante tempo.

| ![](/security-updates/images/Cc708447.note(WS.10).gif)Nota                                                                                                        |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Este documento descreve como sincronizar com as predefinições, mas o WSUS inclui opções que lhe permitem minimizar a utilização de largura de banda durante a sincronização. |

**Para sincronizar o servidor WSUS**
1.  Na consola de Administração do WSUS, seleccione **Sincronizações**.

2.  Clique com o botão direito do rato no painel **Acções** à direita e, em seguida, clique em **Sincronizar agora**.

| ![](/security-updates/images/Cc708447.note(WS.10).gif)Nota                                                                                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se não vir o painel **Acções** no lado direito da consola, na barra de ferramentas da consola clique em **Ver**, clique em **Personalizar** e certifique-se de que a caixa de verificação **Painel de acções** está seleccionada. |

Quando a sincronização estiver concluída, clique em **Actualizações** no painel esquerdo para ver a lista de actualizações.
