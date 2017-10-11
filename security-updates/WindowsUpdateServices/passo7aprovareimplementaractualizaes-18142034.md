---
TOCTitle: 'Passo 7: Aprovar e Implementar Actualizações'
Title: 'Passo 7: Aprovar e Implementar Actualizações'
ms:assetid: '38db25a9-6702-4e43-b536-764e8814afc6'
ms:contentKeyID: 18142034
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720504(v=WS.10)'
---

Passo 7: Aprovar e Implementar Actualizações
============================================

Neste passo, irá aprovar uma actualização para os computadores cliente de teste no grupo Teste. Os computadores no grupo irão registar-se no servidor WSUS durante as 24 horas seguintes. Após este período, poderá utilizar a funcionalidade de relatórios do WSUS para determinar se essas actualizações foram implementadas nos computadores. Se o teste tiver êxito, poderá aprovar a mesma actualização para os restantes computadores na organização.

O Passo 7 contém os seguintes procedimentos:

-   Aprovar e implementar uma actualização.
-   Consultar o relatório de Estado de Actualizações.

**Para aprovar e implementar uma actualização**
1.  Na barra de ferramentas da consola WSUS, clique em **Actualizações**. Por predefinição, a lista de actualizações é filtrada para mostrar apenas Actualizações Críticas e de Segurança que tenham sido aprovadas para detecção em computadores cliente. Utilize o filtro predefinido para este procedimento.

2.  Na lista de actualizações, seleccione as actualizações que pretende aprovar para instalação. O separador **Detalhes** contém informações sobre uma actualização seleccionada. Para seleccionar várias actualizações contíguas, mantenha premida a tecla Shift durante a selecção; para seleccionar várias actualizações não-contíguas, mantenha premida a tecla Ctrl durante a selecção.

3.  Em **Actualizar Tarefas**, clique em **Modificar aprovação**. Aparece a caixa de diálogo **Aprovar Actualizações**.

4.  Na lista **Definições de aprovação de grupo para as actualizações seleccionadas**, clique em **Instalar** na coluna **Aprovação** do grupo Teste e, em seguida, clique em **OK**.

| ![](images/Cc720504.note(WS.10).gif)Nota                                                                                                                                                                |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Existem muitas opções associadas à aprovação de actualizações como, por exemplo, definir prazos e desinstalar actualizações. Estão opções são debatidas na documentação “Microsoft Windows Server Update Services Operations Guide”. |

Após 24 horas, poderá utilizar a funcionalidade de relatórios do WSUS para determinar se essas actualizações foram implementadas nos computadores.

**Par consultar o relatório de Estado de Actualizações**
1.  Na barra de ferramentas da consola WSUS, clique em **Relatórios**.

2.  Na página **Relatórios**, clique em **Estado de Actualizações**.

3.  Se pretender filtrar a lista de actualizações, em **Ver**, seleccione os critérios que pretende utilizar e clique em **Aplicar**.

4.  Se pretender ver o estado de uma actualização por grupo de computadores e, em seguida, por computador, expanda a vista da actualização conforme necessário.

5.  Se pretender imprimir o relatório de Estado de Actualizações, em **Tarefas**, clique em **Imprimir relatório**.

Se as actualizações tiverem sido implementadas com êxito no grupo Teste, poderá aprovar as mesmas actualizações para os restantes computadores na organização.
