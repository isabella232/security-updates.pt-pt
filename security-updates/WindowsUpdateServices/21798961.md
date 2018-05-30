---
TOCTitle: 'Passo 5: Configurar Actualizações de Cliente'
Title: 'Passo 5: Configurar Actualizações de Cliente'
ms:assetid: '5ae60ead-3e94-456c-a692-c0f193ea5d5a'
ms:contentKeyID: 21798961
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Dd939830(v=WS.10)'
---

Passo 5: Configurar Actualizações de Cliente
============================================

No Windows Server Update Services 3.0 (WSUS 3.0 SP2), o Programa de Configuração do WSUS configura automaticamente o IIS para distribuir a versão mais recente do serviço Actualizações Automáticas a cada computador cliente que contacte o servidor WSUS.

A melhor forma de configurar o serviço Actualizações Automáticas depende do ambiente da rede. Num ambiente que utilize o serviço de directório Active Directory®, pode utilizar um Objecto de Política de Grupo (GPO) baseado em domínio, já existente, ou criar um novo GPO. Num ambiente sem o Active Directory, utilize o objecto de Política de Grupo Local. Neste passo, irá configurar as Actualizações Automáticas e apontar os computadores cliente para o servidor WSUS.

Os procedimentos que se seguem assumem que a rede utiliza o Active Directory. Estes procedimentos também assumem que está familiarizado com a Política de Grupo, utilizando-a para gerir a rede.

Para obter mais informações sobre Política de Grupo, consulte o Web site sobre o centro tecnológico de política de grupo [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375).

 
-

Passo 5 Procedimentos
---------------------

No passo 4, concluiu a configuração das actualizações que deseja transferir. Utilize este conjunto de procedimentos para configurar actualizações automáticas para computadores cliente.

1.  Configurar Actualizações Automáticas na Política de Grupo.
2.  Apontar um computador cliente para o servidor WSUS.
3.  Iniciar manualmente a detecção pelo servidor WSUS.

Deve realizar os dois primeiros procedimentos num GPO baseado em domínio à sua escolha e o terceiro procedimento numa linha de comandos no computador cliente.

**Para configurar Actualizações Automáticas**
1.  Na Consola de Gestão da Política de Grupo (GPMC), navegue para o GPO no qual deseja configurar o WSUS e clique em **Editar**.

2.  Na GPMC, expanda **Configuração do Computador**, expanda **Modelos Administrativos**, expanda **Componentes do Windows** e, em seguida, clique em **Windows Update**.

3.  No painel Detalhes, faça duplo clique em **Configurar Actualizações Automáticas**.

4.  Clique em **Activado** e, em seguida, clique numa das seguintes opções:

    -   **Notificar para transferir e notificar para instalar**. Esta opção notifica um administrador com sessão iniciada antes da transferência e antes de instalar as actualizações.
    -   **Transferir automaticamente e notificar para instalar**. Esta opção inicia automaticamente a transferência de actualizações e, em seguida, notifica um administrador com sessão iniciada antes da instalação das actualizações.
    -   **Transferir automaticamente e agendar a instalação**. Esta opção inicia automaticamente a transferência de actualizações e depois instala-as no dia e hora que especificar.
    -   **Permitir ao administrador local escolher a definição**. Esta opção permite que os administradores locais utilizem Actualizações Automáticas no Painel de Controlo para seleccionar uma opção de configuração. Por exemplo, podem escolher a própria data/hora de instalação agendada. Os administradores locais não podem desactivar as Actualizações Automáticas.

5.  Clique em **OK**.

**Para apontar os computadores cliente para o servidor WSUS**
1.  No painel de detalhes do **Windows Update**, faça duplo clique em **Especificar localização do serviço de actualizações da Microsoft na intranet**.

2.  Clique em **Activado** e escreva o URL de HTTP do mesmo servidor WSUS na caixa **Definir o serviço de actualização na intranet para detectar actualizações** e na caixa **Definir o servidor intranet de estatísticas**. Por exemplo, escreva *http://nomeservidor* nas caixas e clique em **OK**.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939830.note(WS.10).gif" />Nota</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Se estiver a utilizar o objecto de Política de Grupo Local para apontar o computador para o WSUS, esta definição será aplicada de imediato e este computador aparece na consola administrativa WSUS pouco tempo depois. Pode acelerar este processo iniciando manualmente um ciclo de detecção.
</td>
</tr>
</tbody>
</table>
 

Depois de configurar um computador cliente, passam alguns minutos antes de o computador aparecer na página **Computadores** na Consola de Administração do WSUS. Para computadores cliente configurados com uma Política de Grupo baseada em domínio, pode ser necessário aguardar cerca de 20 minutos após a Política de Grupo ser actualizada (ou seja, aplica quaisquer novas definições de política ao computador cliente). Por predefinição, a Política de Grupo é actualizada em segundo plano a cada 90 minutos, com um desvio aleatório de 0 a 30 minutos. Se pretender actualizar a Política de Grupo mais cedo, pode ir para uma linha de comandos no computador cliente e escrever **gpupdate /force**.

Para computadores cliente configurados utilizando o GPO Local, a Política de Grupo é aplicada de imediato e a actualização demora cerca de 20 minutos.

Se iniciar a detecção manualmente, não terá de aguardar 20 minutos até que o computador cliente contacte o WSUS.

**Para iniciar manualmente a detecção pelo servidor WSUS**
1.  No computador cliente, clique em **Iniciar** e clique em **Executar**.

2.  Escreva **cmd** na caixa **Abrir** e clique em **OK**.

3.  Na linha de comandos, escreva **wuauclt.exe /detectnow**. Esta opção de linha de comandos indica que o serviço Actualizações Automáticas deverá contactar de imediato o servidor WSUS.

Passo seguinte
--------------

[Passo 6: Configurar Grupos de Computadores](https://technet.microsoft.com/70518732-2179-4e41-9609-7f9999867f41).

Recursos adicionais
-------------------

[Manual Passo a Passo do Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
