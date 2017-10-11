---
TOCTitle: 'Passo 7: Aprovar e Implementar Actualizações no WSUS 3.0'
Title: 'Passo 7: Aprovar e Implementar Actualizações no WSUS 3.0'
ms:assetid: '88fac442-a9d3-4e74-92f6-3822b7237af1'
ms:contentKeyID: 18142200
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc708475(v=WS.10)'
---

Passo 7: Aprovar e Implementar Actualizações no WSUS 3.0
========================================================

Neste passo, irá aprovar uma actualização para os computadores cliente de teste no grupo de testes. Os computadores no grupo irão contactar o servidor WSUS durante as 24 horas seguintes. Após este período, poderá utilizar a funcionalidade de relatórios do WSUS para determinar se essas actualizações foram implementadas nos computadores. Se o teste tiver êxito, poderá aprovar as mesmas actualizações para os restantes computadores na organização.

**O Passo 7 contém os seguintes procedimentos**:

-   Aprovar e implementar uma actualização.
-   Verificar o estado da actualização.

**Para aprovar e implementar uma actualização**
1.  Na consola de Administração do WSUS, clique em **Actualizações**. Desse modo, será apresentado um resumo de actualizações nas vistas predefinidas (**Todas as Actualizações**, **Actualizações Críticas**, **Actualizações de Segurança** e **Actualizações WSUS**). Utilize **Todas as Actualizações** para este procedimento.

2.  Na lista de actualizações, seleccione as actualizações que pretende aprovar para instalação. No painel mais abaixo do painel Actualizações estão disponíveis informações sobre uma actualização seleccionada. Para seleccionar múltiplas actualizações contíguas, mantenha premida a tecla **SHIFT** enquanto clica nas actualizações; para seleccionar múltiplas actualizações não contíguas, mantenha premida a tecla **CTRL** enquanto clica em actualizações.

3.  Clique com o botão direito do rato na selecção e clique em **Aprovar**. É apresentada a caixa de diálogo **Aprovar Actualizações**.

4.  Seleccione um dos grupos (por exemplo, **Teste**) e clique na seta à sua esquerda. Verá um menu de contexto com as opções **Aprovado para Instalação**, **Aprovado para Remoção**, **Não Aprovado**, **Prazo**, **Igual ao Principal** e **Aplicar a Subordinados**. Clique em **Aprovado para Instalação** e, em seguida, clique em **OK**.

5.  Verá uma nova janela, **Progresso da Aprovação**, que mostra o progresso das diferentes tarefas que afectam a aprovação das actualizações. Quando a aprovação estiver concluída, clique em **Fechar** para fechar esta janela.

| ![](images/Cc708475.note(WS.10).gif)Nota                                                      |
|----------------------------------------------------------------------------------------------------------------------------|
| Muitas opções estão associadas à aprovação de actualizações como, por exemplo, definir prazos e desinstalar actualizações. |

Após 24 horas, poderá utilizar a funcionalidade de relatórios do WSUS para determinar se as actualizações foram implementadas nos computadores.

**Para verificar o estado de uma actualização**
1.  Na consola de Administração do WSUS, clique em **Relatórios** no painel esquerdo.

2.  Na página **Relatórios**, verá um número de relatórios uniformizados. Clique no relatório **Actualizar Resumo de Estado**. Verá a janela **Relatório de Actualizações**.

3.  Se pretender filtrar a lista de actualizações, seleccione os critérios que pretende utilizar (por exemplo, **Incluir actualizações nestas classificações**) e, em seguida, clique em **Executar Relatório** na barra de ferramentas da janela.

4.  Verá o painel **Relatório de Actualizações**. Pode verificar o estado de actualizações individuais seleccionando a actualização na secção esquerda do painel. A última secção do painel do relatório mostra o resumo do estado da actualização.

5.  Pode guardar ou imprimir este relatório clicando no ícone apropriado na barra de ferramentas.

Se as actualizações tiverem sido implementadas com êxito no grupo de testes, poderá aprová-las para os restantes computadores na organização.
