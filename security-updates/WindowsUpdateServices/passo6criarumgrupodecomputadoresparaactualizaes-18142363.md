---
TOCTitle: 'Passo 6: Criar um Grupo de Computadores para Actualizações'
Title: 'Passo 6: Criar um Grupo de Computadores para Actualizações'
ms:assetid: 'fe219654-eae8-45ca-a44b-c1e05c3c3e93'
ms:contentKeyID: 18142363
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc708629(v=WS.10)'
---

Passo 6: Criar um Grupo de Computadores para Actualizações
==========================================================

Os grupos de computadores são uma parte importante das implementações do WSUS, mesmo que se trate de uma implementação básica. Os grupos de computadores permitem-lhe definir computadores específicos como alvos de actualizações. Existem dois grupos de computadores predefinidos: Todos os Computadores e Computadores Não Atribuídos. Por predefinição, quando cada computador cliente contacta inicialmente o servidor WSUS, o servidor adiciona o computador cliente a cada um destes grupos.

É possível criar grupos de computadores personalizados. Uma vantagem da criação de grupos de computadores consiste em permitir-lhe testar as actualizações antes de as implementar amplamente. Se os testes correrem bem, poderá expandir as actualizações ao grupo Todos os Computadores. Não há limite quanto ao número de grupos personalizados que pode criar.

**Para configurar grupos de computadores**
1.  Especifique a forma de atribuição de computadores a grupos de computadores. Existem duas opções: direccionamento do lado do cliente e direccionamento do lado do servidor A opção de direccionamento do lado do servidor envolve a adição manual de cada computador ao respectivo grupo utilizando-se o WSUS. A opção de direccionamento do lado do cliente envolve a adição automática dos clientes utilizando-se a Política de Grupo ou chaves de registo.

2.  Crie o grupo de computadores no WSUS.

3.  Mova os computadores para grupos, utilizando o método escolhido no passo 1.

Esta secção explica como utilizar o direccionamento do lado do servidor e mover manualmente computadores para os respectivos grupos utilizando a consola de Administração do WSUS. Se tiver múltiplos computadores cliente a atribuir a grupos de computadores, pode utilizar o direccionamento do lado do cliente, o que automatiza o movimentação dos computadores para grupos de computadores.

Pode utilizar o Passo 6 para configurar um grupo de teste que contenha pelo menos um computador de teste.

**O Passo 6 contém os seguintes procedimentos:**

-   Criar um grupo.
-   Adicionar um computador ao grupo.

**Para criar um grupo**
1.  Na consola de Administração do WSUS, expanda **Computadores** e seleccione **Todos os Computadores**.

2.  Clique com o botão direito do rato em **Todos os Computadores** ou vá para o painel **Acções** e, em seguida, clique em **Adicionar Grupo de Computadores**.

3.  Verá uma caixa de diálogo **Adicionar Grupo de Computadores**. Especifique o nome do novo grupo.

Utilize o próximo procedimento para atribuir um computador cliente ao grupo de teste. Um computador cliente apropriado para testes é qualquer computador com software e hardware indicativo da maioria de computadores na rede, mas não um computador atribuído a uma função crítica. Desta forma, poderá saber de que forma os computadores semelhantes ao computador de teste irão lidar com as actualizações aprovadas.

**Para adicionar um computador ao grupo**
1.  Na consola de Administração do WSUS, clique em **Computadores**.

2.  Clique no grupo do computador que pretende mover.

3.  Na lista de computadores, seleccione o computador que pretende mover.

4.  Clique com o botão direito do rato em **Alterar Membros**.

5.  Verá uma caixa de diálogo, **Definir Membros de Grupo de Computadores**, com uma lista de grupos.

6.  Verifique o grupo para o qual pretende mover o computador e, em seguida, clique em **OK**.
