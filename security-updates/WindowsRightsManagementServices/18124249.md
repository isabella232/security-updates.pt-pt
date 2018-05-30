---
TOCTitle: Para Configurar um Grupo de Super Utilizadores
Title: Para Configurar um Grupo de Super Utilizadores
ms:assetid: 'f2ef847e-2824-471f-9079-5c343094aba8'
ms:contentKeyID: 18124249
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747798(v=WS.10)'
---

Para Configurar um Grupo de Super Utilizadores
==============================================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

Antes de ser designado como grupo de super utilizadores para o RMS, o grupo já deve existir no Active Directory e as propriedades desse grupo devem incluir um endereço de correio electrónico (especificado como um nome de domínio totalmente qualificado) que seja igual ao do nome da conta.

Configurar um Grupo de Super Utilizadores
-----------------------------------------

#### Para Configurar um Grupo de Super Utilizadores

1.  Abra a página **Administração Global** e, em seguida, no Web site em que pretende definir um grupo de super utilizadores, clique em **Administrar o RMS neste Web site**.

2.  Na área **Ligações da administração**, clique em **Definições de segurança**.

3.  Na área **Super utilizadores**, clique em **Activar**, para adicionar um grupo de super utilizadores.

4.  Em **Nome do grupo de super utilizadores**, escreva o nome completo do domínio qualificado, sob a forma *nome\_grupo*@*nome\_domínio.com*, de um grupo existente nesta floresta do Active Directory a cujos membros vão ser concedidos direitos de proprietário para todos os documentos protegidos pelo RMS e, em seguida, clique em **Guardar**.

    Para desactivar os direitos para o grupo de super utilizadores, clique em **Desactivar**.

Para mais informações sobre a execução deste procedimento, consulte "[Utilizar o Grupo de Super Utilizadores](https://technet.microsoft.com/0febcb3e-7124-4e51-971a-1013b928d33b)" anteriormente nesta secção.
