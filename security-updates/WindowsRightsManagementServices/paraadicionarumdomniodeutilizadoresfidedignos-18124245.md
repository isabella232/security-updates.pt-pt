---
TOCTitle: Para Adicionar um Domínio de Utilizadores Fidedignos
Title: Para Adicionar um Domínio de Utilizadores Fidedignos
ms:assetid: 'ed672e58-6272-4ac0-a434-d1d938037e93'
ms:contentKeyID: 18124245
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747793(v=WS.10)'
---

Para Adicionar um Domínio de Utilizadores Fidedignos
====================================================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

Adicionar um Domínio de Utilizador Fidedigno
--------------------------------------------

#### Para Adicionar um Domínio de Utilizadores Fidedignos

1.  Abra a página **Administração Global** e, em seguida, no Web site em que pretende adicionar um domínio de utilizadores fidedignos, clique em **Administrar o RMS neste Web site**.

2.  Na área de ligações **Administração**, clique em **Políticas de fidedignidade**.

3.  Na área **Domínios de utilizadores fidedignos**, clique em **Procurar**, localize e faça duplo clique no certificado de licenciador de servidores do domínio de utilizadores que pretende importar para estabelecer uma relação fidedigna e, em seguida, clique em **Adicionar**.

    O nome do domínio aparece na lista **Domínios de utilizadores fidedignos**.

4.  Para especificar, dentro do domínio de utilizadores fidedignos, quais os domínios de correio electrónico que são considerados fidedignos, clique em **Domínios fidedignos**, junto do nome do certificado na lista, para abrir a janela **Domínios de correio electrónico fidedignos**.

5.  Escolha uma das seguintes opções de fidedignidade:

    -   Seleccione a opção **Considerar fidedignos todos os domínios de correio electrónico**, para considerar fidedignas todas as contas de utilizador pertencentes a esse domínio.
        –ou-
    -   Seleccione a opção **Considerar fidedignos apenas os domínios de correio electrónico especificados** e, em seguida, escreva o nome do domínio a ser considerado fidedigno, como exemplo.com e, em seguida, clique em **Adicionar**. Desta forma adiciona o domínio à lista Domínios de correio electrónico fidedignos. Para remover um nome da lista, seleccione o nome e, em seguida, clique em **Remover**. A listagem de um domínio inclui todos os respectivos subdomínios.

6.  Se está a utilizar o RMS num ambiente em que necessita de expandir os membros do grupo por florestas, seleccione a caixa de verificação **Considerar fidedigno o licenciamento do RM de identificadores de segurança (SID) para este domínio de utilizador**.

7.  Quando concluir, clique em **Fechar a janela e voltar às políticas de fidedignidade**.

Para mais informações sobre como efectuar este procedimento, consulte "[Adicionar e Remover Domínios de Utilizadores Fidedignos](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)" anteriormente nesta secção.
