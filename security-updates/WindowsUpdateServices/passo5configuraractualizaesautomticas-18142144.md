---
TOCTitle: 'Passo 5: Configurar Actualizações Automáticas'
Title: 'Passo 5: Configurar Actualizações Automáticas'
ms:assetid: '5da6d10a-6ff1-4de8-b53a-4893bf8bd9fa'
ms:contentKeyID: 18142144
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720532(v=WS.10)'
---

Passo 5: Configurar Actualizações Automáticas
=============================================

Os computadores cliente WSUS requerem uma versão compatível do serviço Actualizações Automáticas. O Programa de Configuração do WSUS configura o IIS para distribuir a versão mais recente do serviço Actualizações Automáticas a cada computador cliente que contacte o servidor WSUS.

A melhor forma de configurar o serviço Actualizações Automáticas depende do ambiente da rede. Num ambiente com o Active Directory, pode utilizar um GPO (Group Policy Object) baseado em domínio. Num ambiente sem o Active Directory, utilize o objecto de Política de Grupo Local. Quer utilize o GPO Local ou um GPO armazenado num GPO baseado em domínio, terá de apontar os computadores cliente para o servidor WSUS e, em seguida, configurar o serviço Actualizações Automáticas.

As instruções que se seguem assumem que a rede executa o Active Directory. Estes procedimentos também assumem que está familiarizado com a Política de Grupo, utilizando-a para gerir a rede. É necessário criar um novo GPO para definições WSUS e ligar esse GPO ao domínio.

Para obter mais informações sobre Política de Grupo, consulte o Web site sobre o centro tecnológico de política de grupo ([http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375)). (Esta página poderá estar em inglês.)

**O Passo 5 contém os seguintes procedimentos**:

-   Adicionar o Modelo Administrativo do WSUS.
-   Configurar o serviço Actualizações Automáticas.
-   Apontar o computador cliente para o servidor WSUS.
-   Iniciar manualmente a detecção pelo servidor WSUS.

Efectue os três primeiros procedimentos num objecto de Política de Grupo baseado em domínio. Será necessário criar um novo GPO ou utilizar um GPO existente. Se utilizar uma GPMC (Group Policy Management Console) para gerir os GPOs, navegue para o GPO que pretende modificar e, em seguida, clique em **Editar**.

Para poder ver definições de política para gerir o WSUS, será necessário garantir que o ficheiro de modelo administrativo WSUS, o wuau.adm, é adicionado ao Editor de Objecto de Política de Grupo. Como, por predefinição, o wuau.adm é disponibilizado pelo sistema operativo, deve estar presente no Editor de Objecto de Política de Grupo.

**Para adicionar o Modelo Administrativo do WSUS**
1.  No Editor de Objecto de Política de Grupo, clique em qualquer um dos nós **Modelos Administrativos** .

2.  No menu **Acção** , clique em **Adicionar/Remover Modelos** e, em seguida, clique em **Adicionar**.

3.  Na caixa de diálogo **Modelos de Políticas**, clique em **wuau.adm**e, em seguida, clique em **Abrir**.

4.  Na caixa de diálogo **Adicionar/Remover Modelos**, clique em **Fechar**.

**Para configurar Actualizações Automáticas**
1.  No Editor de Objecto de Política de Grupo, expanda **Configuração do Computador**, expanda **Modelos Administrativos**, expanda **Componentes do Windows** e, em seguida, clique em **Windows Update**.

2.  No painel de detalhes, faça duplo clique em **Configurar Actualizações Automáticas**.

3.  Clique em **Activado** e, em seguida, clique numa das seguintes opções:

    -   **Notificar para transferir e notificar para instalar**: Esta opção notifica um administrador com sessão iniciada antes da transferência e antes da instalação das actualizações.
    -   **Transferir automaticamente e notificar para instalar**: Esta opção inicia automaticamente a transferência de actualizações e, em seguida, notifica um administrador com sessão iniciada antes da instalação das actualizações.
    -   **Transferir automaticamente e agendar a instalação**: Se a opção Actualizações Automáticas estiver configurada para efectuar uma instalação agendada, terá também de definir o dia e a hora para a instalação agendada periódica.
    -   **Permitir ao administrador local escolher a definição**: Com esta opção, os administradores locais têm permissão para utilizar Actualizações Automáticas no Painel de Controlo para seleccionar uma opção de configuração à escolha. Por exemplo, podem escolher a própria data/hora de instalação agendada. Os administradores locais não têm permissão para desactivar Actualizações Automáticas.

4.  Clique em **OK**.

| ![](images/Cc720532.note(WS.10).gif)Nota                                                                                                                 |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A definição **Permitir ao administrador local escolher a definição** só aparece se o serviço Actualizações Automáticas se tiver auto-actualizado para a versão compatível com o WSUS. |

**Para apontar o computador cliente para o servidor WSUS**
1.  No Editor de Objecto de Política de Grupo, expanda **Configuração do Computador**, expanda **Modelos Administrativos**, expanda **Componentes do Windows** e, em seguida, clique em **Windows Update**.

2.  No painel de detalhes, faça duplo clique em **Especificar localização do serviço do Windows Update na intranet**.

3.  Clique em **Activado**e escreva o URL de HTTP do mesmo servidor WSUS na caixa **Defina o serviço de actualização na intranet para detectar actualizações** e na caixa **Defina o servidor de estatísticas na intranet** . Por exemplo, escreva *http://nomeservidor* em ambas as caixas e, em seguida, clique em **OK**.

| ![](images/Cc720532.note(WS.10).gif)Nota                                                                                                                                                                                                                                      |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se estiver a utilizar o objecto de Política de Grupo Local para apontar este computador para o WSUS, esta definição será aplicada de imediato e este computador deverá aparecer na consola administrativa WSUS pouco tempo depois. Pode acelerar este processo iniciando manualmente um ciclo de detecção. |

Após a configuração de um computador cliente, será necessário aguardar alguns minutos até que o mesmo apareça na página **Computadores** da consola WSUS. Para computadores cliente configurados com uma Política de Grupo baseada em domínio, será necessário aguardar cerca de 20 minutos após a Política de Grupo ser actualizada (ou seja, aplica quaisquer novas definições de política ao computador cliente). Por predefinição, a Política de Grupo é actualizada em segundo plano a cada 90 minutos, com um desvio aleatório de 0 a 30 minutos. Se pretender actualizar a Política de Grupo mais cedo, pode ir para uma linha de comandos no computador cliente e escrever: **gpupdate /force**.

Para computadores cliente configurados com o GPO Local, a Política de Grupo é aplicada de imediato e a actualização irá demorar cerca de 20 minutos.

Depois de a Política de Grupo ser aplicada, poderá iniciar manualmente a detecção. Se iniciar a detecção manualmente, não terá de aguardar 20 minutos até que o computador cliente contacte o WSUS.

**Para iniciar manualmente a detecção pelo servidor WSUS**
1.  Na computador cliente, clique em **Iniciar** e, em seguida, clique em **Executar**.

2.  Escreva **cmd** na caixa **Abrir** e, em seguida, clique em **OK**.

3.  Na linha de comandos, escreva **wuauclt.exe /detectnow**. Esta opção de linha de comandos indica que o serviço Actualizações Automáticas deverá contactar de imediato o servidor WSUS.
