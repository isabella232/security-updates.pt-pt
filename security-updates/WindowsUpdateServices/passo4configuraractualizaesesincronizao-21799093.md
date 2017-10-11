---
TOCTitle: 'Passo 4: Configurar Actualizações e Sincronização'
Title: 'Passo 4: Configurar Actualizações e Sincronização'
ms:assetid: 'deeaa7e1-9b50-45cb-9537-d75f70de3405'
ms:contentKeyID: 21799093
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Dd939924(v=WS.10)'
---

Passo 4: Configurar Actualizações e Sincronização
=================================================

Esta secção descreve como configurar um conjunto de actualizações que queira transferir utilizando o Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2).

Passo 4 Procedimentos
---------------------

Pode realizar estes procedimentos utilizando o Assistente de Configuração do WSUS ou a Consola de Administração do WSUS.

1.  Guardar e transferir informações sobre o servidor a montante e o servidor proxy.
2.  Escolher o idioma das actualizações.
3.  Seleccionar os produtos para os quais pretende receber actualizações.
4.  Escolher as classificações das actualizações.
5.  Especificar a agenda de sincronização para este servidor.

Depois de configurar a ligação de rede, poderá transferir actualizações através da sincronização do servidor WSUS. A sincronização começa quando o servidor WSUS contacta o Microsoft Update. Após o contacto, o WSUS determina se foram disponibilizadas novas actualizações desde a última sincronização. Quando sincroniza o servidor WSUS pela primeira vez, todas as actualizações se encontram disponíveis e preparadas para aprovação para instalação. A sincronização inicial pode demorar bastante tempo.

Os procedimentos desta secção descrevem a sincronização com as predefinições. O WSUS 3.0 SP2 inclui também opções que lhe permitem minimizar a utilização de largura de banda durante a sincronização.

Se estiver a utilizar o Assistente de Configuração do Windows Server Update Services
------------------------------------------------------------------------------------

Nos procedimentos do passo 3, concluiu a configuração do servidor a montante e do servidor proxy. Este novo conjunto de procedimentos começa na página **Ligar ao Servidor a Montante** desse assistente de configuração.

**Para guardar e transferir informações sobre o servidor a montante e o servidor proxy**
1.  Na página Ligar ao Servidor a Montante do assistente de configuração, clique no botão **Iniciar Ligação**. Esta acção guarda e carrega as suas definições e recolhe simultaneamente informações acerca das actualizações disponíveis.

2.  Enquanto a ligação estiver a ser estabelecida, o botão **Parar Ligação** ficará disponível. Se existirem problemas com a ligação, clique em **Parar Ligação**, corrija os problemas e reinicie a ligação.

3.  Depois de a transferência ter sido concluída com êxito, clique em **Seguinte**.

**Para escolher idiomas de actualização**
1.  A página Escolher Idiomas permite receber actualizações a partir de todos os idiomas ou de um subconjunto de idiomas. A selecção de um subconjunto de idiomas poupa espaço em disco, mas é importante que escolha todos os idiomas que serão necessários por todos os clientes deste servidor WSUS.

    Se optar por obter actualizações apenas para idiomas específicos, seleccione **Transferir actualizações apenas nestes idiomas** e seleccione os idiomas para os quais pretende actualizações.

2.  Clique em **Seguinte**.

**Para escolher produtos de actualização**
1.  A página Escolher Produtos permite especificar os produtos para os quais pretende actualizações. Seleccione categorias de produto, tal como o Windows, ou produtos específicos, tal como o Windows Server 2008. A selecção de uma categoria irá fazer com que todos os produtos dessa categoria sejam seleccionados.

2.  Clique em **Seguinte**.

**Para escolher classificações de actualização**
1.  A página Escolher Classificações permite especificar as classificações de actualizações que pretende obter. Escolha todas as classificações ou um subconjunto das mesmas.

2.  Clique em **Seguinte**

**Para configurar a agenda de sincronização**
1.  Na página Definir Agenda de Sincronização, escolhe se vai efectuar a sincronização de forma manual ou automática.

    Se escolher **Sincronizar manualmente**, terá de iniciar o processo de sincronização a partir da Consola de Administração do WSUS.

    Se escolher **Sincronizar automaticamente**, o servidor WSUS será sincronizado a intervalos especificados. Defina a hora da **Primeira sincronização** e especifique o número de **Sincronizações por dia** que pretende que este servidor efectue. Por exemplo, se especificar a execução de quatro sincronizações por dia, com início às 03:00, as sincronizações terão lugar às 03:00, 09:00, 15:00 e 21:00.

2.  Clique em **Seguinte**.

3.  Na página Concluído, pode iniciar a Consola de Administração do WSUS deixando seleccionada a caixa de verificação **Iniciar o snap-in de Administração do Windows Server Update Services** e pode iniciar a primeira sincronização deixando seleccionada a caixa de verificação **Iniciar sincronização inicial**.

4.  Clique em **Concluir**.

 
    <table style="border:1px solid black;">
    <colgroup>
    <col width="100%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th style="border:1px solid black;" ><img src="images/Dd939924.Important(WS.10).gif" />Importante</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td style="border:1px solid black;">Não é possível guardar alterações de configuração efectuadas durante a sincronização do servidor. Aguarde até a sincronização ter terminado e, depois, efectue as alterações.
    </td>
    </tr>
    </tbody>
    </table>
 

Se estiver a utilizar a Consola de Administração do WSUS
--------------------------------------------------------

Os procedimentos que se seguem explicam como realizar os passos de configuração utilizando a Consola de Administração do WSUS.

**Para escolher produtos e actualizar classificações**
1.  No painel **Opções**, clique em **Produtos e Classificações**. Aparece uma caixa de diálogo com os separadores **Produtos** e **Classificações**.

2.  No separador **Produtos**, seleccione a categoria de produto ou os produtos específicos para os quais pretende que este servidor receba actualizações, ou seleccione **Todos os Produtos**.

3.  No separador **Classificações**, seleccione as classificações de actualizações pretendidas ou seleccione **Todas as Classificações**.

4.  Clique em **OK** para guardar as selecções.

**Para escolher idiomas e ficheiros de actualização**
1.  No painel **Opções**, clique em **Idiomas e Ficheiros de Actualização**. Aparece uma caixa de diálogo com os separadores **Ficheiros de Actualização** e **Idiomas de Actualização**.

2.  No separador **Ficheiros de Actualização**, escolha se pretende **Armazenar ficheiros de actualização localmente neste servidor** ou definir que todos os computadores cliente instalem a partir do Microsoft Update. Se optar por armazenar os ficheiros de actualização neste servidor, terá igualmente de decidir se transfere apenas as actualizações aprovadas ou se transfere ficheiros de instalação rápida.

3.  No separador **Idiomas de Actualização**, se estiver a armazenar ficheiros de actualização localmente, pode escolher entre **Transferir actualizações em todos os idiomas** (predefinido) ou **Transferir actualizações apenas nos idiomas especificados**. Se este servidor WSUS tiver servidores a jusante, irá receber actualizações apenas nos idiomas especificados pelo servidor a montante.

4.  Clique em **OK** para guardar estas definições.

**Para sincronizar o servidor WSUS**
1.  No painel **Opções**, clique em **Agenda de Sincronização**.

2.  No separador **Agenda de Sincronização**, escolha se vai efectuar a sincronização de forma manual ou automática.

    Se escolher **Sincronizar manualmente**, terá de iniciar o processo de sincronização a partir da Consola de Administração do WSUS.

    Se escolher **Sincronizar automaticamente**, o servidor WSUS será sincronizado a intervalos especificados. Defina a hora da **Primeira sincronização** e especifique o número de **Sincronizações por dia** que pretende que este servidor efectue. Por exemplo, se especificar a execução de quatro sincronizações por dia, com início às 03:00, as sincronizações terão lugar às 03:00, 09:00, 15:00 e 21:00.

3.  Clique em **OK** para guardar as selecções.

4.  No painel de navegação da Consola de Administração do WSUS, seleccione **Sincronizações**.

5.  Clique com o botão direito do rato ou vá para o painel **Acções** à direita e, em seguida, clique em **Sincronizar agora**.

    Se não vir o painel **Acções** no lado direito da consola, na barra de ferramentas da consola clique em **Ver**, clique em **Personalizar** e certifique-se de que a caixa de verificação **Painel de acções** está seleccionada.

6.  Quando a sincronização estiver concluída, clique em **Actualizações** no painel esquerdo para ver a lista de actualizações.

Passo seguinte
--------------

[Passo 5: Configurar Actualizações de Cliente](https://technet.microsoft.com/5ae60ead-3e94-456c-a692-c0f193ea5d5a).

Recursos adicionais
-------------------

[Manual Passo a Passo do Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
