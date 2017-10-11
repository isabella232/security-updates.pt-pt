---
TOCTitle: 'Passo 5: Actualizar e Configurar Actualizações Automáticas'
Title: 'Passo 5: Actualizar e Configurar Actualizações Automáticas'
ms:assetid: '4ac8d574-f48e-4d9d-86c9-9aeb0f57e750'
ms:contentKeyID: 18142051
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720533(v=WS.10)'
---

Passo 5: Actualizar e Configurar Actualizações Automáticas
==========================================================

Os computadores cliente WSUS requerem uma versão compatível do serviço Actualizações Automáticas. O Programa de Configuração do WSUS configura o IIS para distribuir a versão mais recente do serviço Actualizações Automáticas a cada computador cliente que contacte o servidor WSUS.

| ![](images/Cc720533.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Embora a maioria das versões do serviço Actualizações Automáticas possa ser apontada para o servidor WSUS, actualizando-se automaticamente para a versão compatível com WSUS, a versão de Actualizações Automáticas incluída no Windows XP sem service packs não consegue actualizar-se automaticamente. Se tiver o Windows XP sem service packs no ambiente e nunca tiver utilizado o Software Update Services (SUS), consulte a documentação “Deploying Microsoft Windows Server Update Services” para obter instruções. |

A melhor forma de configurar o serviço Actualizações Automáticas depende do ambiente da rede. Num ambiente Active Directory, pode utilizar um objecto de Política de Grupo (GPO, *Group Policy object*) baseado no Active Directory. Num ambiente não-Active Directory, utilize o objecto de Política de Grupo local. Quer utilize o GPO Local ou um GPO armazenado num controlador de domínio, terá de apontar os computadores cliente para o servidor WSUS e configurar em seguida o serviço Actualizações Automáticas.

As instruções que se seguem assume que a rede executa o Active Directory. Estes procedimentos também assumem que já configurou e está familiarizado com a Política de Grupo, utilizando-a para gerir a rede. É necessário criar um novo GPO para definições WSUS e ligar esse GPO ao nível do domínio.

Para mais informações sobre Política de Grupo, consulte a [página sobre Política de Grupo](http://go.microsoft.com/fwlink/?linkid=47375) em http://go.microsoft.com/fwlink/?LinkID=47375 (o documento pode estar disponível apenas em inglês).

O Passo 5 contém os seguintes procedimentos:

-   Carregar o Modelo Administrativo do WSUS.
-   Configurar o serviço Actualizações Automáticas.
-   Apontar computadores cliente para o servidor WSUS.
-   Iniciar manualmente detecção no computador cliente.

Efectue os três procedimentos seguintes num objecto de Política de Grupo baseado no Active Directory.

**Para adicionar o Modelo Administrativo do WSUS**
1.  No Editor de Objectos de Política de Grupo, clique em qualquer um dos nós **Modelos Administrativos**.

2.  No menu **Acção**, clique em **Adicionar/Remover Modelos**.

3.  Clique em **Adicionar**.

4.  Na caixa de diálogo **Modelos de Políticas**, clique em **wuau.adm** e clique em **Abrir**.

5.  Na caixa de diálogo **Adicionar/Remover Modelos**, clique em **Fechar**.

**Para configurar o comportamento de Actualizações Automáticas**
1.  No Editor de Objectos de Política de Grupo, expanda **Configuração do Computador**, expanda **Modelos Administrativos**, expanda **Componentes do Windows** e clique em **Windows Update**.

2.  No painel de detalhes, faça duplo clique em **Configurar Actualizações Automáticas**.

3.  Clique em **Activado** e, em seguida, clique numa das opções seguintes:

    -   **Notificar para transferir e notificar para instalar.** Esta opção notifica um administrador com sessão iniciada antes da transferência e antes da instalação das actualizações.
    -   **Transferir automaticamente e notificar para instalar.** Esta opção inicia automaticamente a transferência de actualizações e notifica um administrador com sessão iniciada antes da instalação das actualizações.
    -   **Transferir automaticamente e agendar a instalação.** Se a opção Actualizações Automáticas estiver configurada para efectuar uma instalação agendada, terá também de definir o dia e a hora para a instalação agendada periódica.
    -   **Permitir ao administrador local escolher a definição.** Com esta opção, os administradores locais têm permissão para utilizar Actualizações Automáticas no Painel de Controlo para seleccionar uma opção de configuração à escolha. Por exemplo, podem escolher a própria data/hora de instalação agendada. Os administradores locais não têm permissão para desactivar Actualizações Automáticas.

4.  Clique em **OK**.

| ![](images/Cc720533.note(WS.10).gif)Nota                                                                                                                 |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A definição **Permitir ao administrador local escolher a definição** só aparece se o serviço Actualizações Automáticas se tiver auto-actualizado para a versão compatível com o WSUS. |

**Para apontar o computador cliente para o servidor WSUS**
1.  No Editor de Objectos de Política de Grupo, expanda **Configuração do Computador**, expanda **Modelos Administrativos**, expanda **Componentes do Windows** e clique em **Windows Update**.

2.  No painel de detalhes, faça duplo clique em **Especificar localização do serviço do Windows Update na intranet**.

3.  Clique em **Activado** e escreva o URL HTTP do mesmo servidor WSUS na caixa **Definir o serviço de actualização na intranet para detectar actualizações** e na caixa **Definir o servidor intranet de estatísticas**. Por exemplo, escreva **http://***nomeservidor* em ambas as caixas.

4.  Clique em **OK**.

| ![](images/Cc720533.note(WS.10).gif)Nota                                                                                                                                                                                                                                          |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se estiver a utilizar o objecto de Política de Grupo Local para apontar este computador para o WSUS, esta definição será aplicada de imediato e este computador deverá aparecer na consola administrativa WSUS em cerca de 20 minutos. Pode acelerar este processo iniciando manualmente um ciclo de detecção. |

Após a configuração de um computador cliente, será necessário aguardar alguns minutos até que o mesmo apareça na página **Computadores** na consola WSUS. Para computadores cliente configurados com um GPO baseado no Active Directory, será necessário aguardar cerca de 20 minutos após a Política de Grupo ser actualizada (ou seja, aplica toda e qualquer nova definição ao computador cliente). Por predefinição, a Política de Grupo é actualizada em segundo plano a cada 90 minutos, com um desvio aleatório de 0 a 30 minutos. Se pretender actualizar a Política de Grupo mais cedo, pode ir para uma linha de comandos no computador cliente e escrever: **gpupdate /force**.

Para computadores cliente configurados com o GPO Local, a Política de Grupo é aplicada de imediato, sendo necessário aguardar cerca de 20 minutos.

Assim que a Política de Grupo seja aplicada, poderá iniciar manualmente a detecção. Se efectuar este passo, não terá de aguardar 20 minutos até que o computador cliente contacte o WSUS.

**Para iniciar manualmente a detecção pelo servidor WSUS**
1.  No computador cliente, clique em **Iniciar** e, em seguida, clique em **Executar**.

2.  Escreva **cmd** e clique em **OK**.

3.  Na linha de comandos, escreva **wuauclt.exe /detectnow**. Esta opção de linha de comandos indica que o serviço Actualizações Automáticas deverá contactar de imediato o servidor WSUS.
