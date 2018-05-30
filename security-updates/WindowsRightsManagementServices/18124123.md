---
TOCTitle: Para Desinstalar o RMS
Title: Para Desinstalar o RMS
ms:assetid: '885e3b4f-ea32-466f-9f7f-d8440b0f7c28'
ms:contentKeyID: 18124123
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747587(v=WS.10)'
---

Para Desinstalar o RMS
======================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

Desinstalar o RMS
-----------------

#### Para Desinstalar o RMS

1.  Inicie a sessão no servidor em que pretende desinstalar o RMS.

    | ![](/security-updates/images/Cc747587.Important(WS.10).gif)Importante                                                                                                                                                                                                                                      |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Se estiver a remover o RMS de um servidor no cluster de certificações de raiz, deve começar por o desaprovisionar através da página **Administração Global**, clicando em **Remover o RMS deste Web site**. Não necessita de desaprovisionar um servidor de licenciamentos antes de desinstalar o RMS desse servidor. |

2.  Abra **Adicionar ou Remover Programas** no **Painel de Controlo**.

3.  Na caixa de diálogo **Adicionar ou remover programas**, clique em **Serviços de Gestão de Direitos do Windows** e, em seguida, clique em **Remover** para remover o RMS SP1.
