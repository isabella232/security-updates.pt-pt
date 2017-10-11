---
TOCTitle: Para Activar a Administração Remota do RMS
Title: Para Activar a Administração Remota do RMS
ms:assetid: '00f17054-5f5d-47e2-89c1-7a593b930bb3'
ms:contentKeyID: 18123927
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720181(v=WS.10)'
---

Para Activar a Administração Remota do RMS
==========================================

O Internet Explorer 6.0 ou posterior deve estar instalado no computador que estiver a ser utilizado para a administração remota do RMS.

Activar a Administração Remota do RMS
-------------------------------------

#### Para Activar a Administração Remota do RMS

1.  Inicie sessão no servidor que pretende administrar remotamente.

2.  Nas **Ferramentas administrativas**, abra o snap-in **Gestor de Serviços de Informação Internet (IIS)**.

3.  Expanda o item que representa o Web site no qual aprovisionou o RMS.

4.  Clique com o botão direito do rato na pasta **\_wmcs** e, em seguida, clique em **Propriedades**. No separador **Segurança de directório**, em **Comunicações seguras**, clique em **Editar**, em **Exigir canal seguro (SSL)** e, em seguida, clique em **OK**. Isto aplica a protecção Secure Sockets Layer (SSL) aos serviços Web do RMS. Para mais informações sobre como gerir Web sites utilizando o IIS, consulte a ajuda do IIS.

    | ![](images/Cc720181.Important(WS.10).gif)Importante                                                                                                                                                                                              |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Pode proteger os serviços Web do RMS com o SSL para maior segurança e para activar o acesso HTTP remoto às páginas de Web da administração do RMS. Se pretender activar o SSL para os serviços Web do RMS, obtenha e instale um certificado de servidor da Web de SSL válido. |

5.  Clique com o botão direito do rato na pasta **Admin** e, em seguida, clique em **Propriedades**. No separador **Segurança de directório**, em **Restrições de endereço IP e de nome de domínio**, clique em **Editar** e, em seguida, em **Restrições de acesso de endereço IP**, clique em **Acesso concedido**, para que todos os computadores possam pedir uma ligação a este Web site.
