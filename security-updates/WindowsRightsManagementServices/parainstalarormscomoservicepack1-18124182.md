---
TOCTitle: Para Instalar o RMS com o Service Pack 1
Title: Para Instalar o RMS com o Service Pack 1
ms:assetid: 'dab20175-a690-43f8-b943-768d289daa0d'
ms:contentKeyID: 18124182
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747689(v=WS.10)'
---

Para Instalar o RMS com o Service Pack 1
========================================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

O computador em que está a instalar o RMS deve ser um servidor membro num domínio ou ser um controlador de domínio. Não é possível implementar o RMS num servidor autónomo num grupo de trabalho.

| ![](/security-updates/images/Cc747689.Important(WS.10).gif)Importante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Não aprovisione o RMS em qualquer outro servidor enquanto não concluir a instalação e o aprovisionamento do primeiro servidor de certificações de raiz. Para obter instruções, consulte "[Para Aprovisionar o Primeiro Servidor de Certificações de Raiz](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)", "[Para Aprovisionar um Servidor de Licenciamento](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)" ou "[Para Adicionar um Servidor a um Cluster](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)" posteriormente nesta secção. |

| ![](/security-updates/images/Cc747689.Important(WS.10).gif)Importante                                                                                                                                                                         |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| O RMS SP1 pode ser instalado num servidor que esteja a utilizar uma versão anterior do RMS. No entanto, se desactivou o RMS, este deve ser completamente removido utilizando a função Adicionar ou Remover Programas antes de tentar instalar o RMS SP1. |

Instalar o RMS com o Service Pack 1
-----------------------------------

#### Para Instalar o RMS com o Service Pack 1

1.  No servidor, no qual deseja instalar o RMS SP1, inicie a sessão com uma conta de domínio que seja membro do grupo de administradores local.

2.  Quando a caixa de diálogo **Bem-vindo** aparecer, reveja a lista de software a ser instalado e, depois, clique em **Seguinte**.

3.  Na caixa de diálogo **Contrato de licença**, reveja o contrato, seleccione **Concordo** e clique em **Seguinte**.

4.  Em **Pasta**, aceite a pasta predefinida ou especifique outra pasta e clique em **Seguinte**.

5.  Na caixa de diálogo **Confirmar instalação**, clique em **Instalar** para iniciar a instalação.

6.  Quando a caixa de diálogo **Instalação concluída** aparecer, clique em **Fechar**.

    | ![](/security-updates/images/Cc747689.note(WS.10).gif)Nota                                                                                 |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Se aparecer uma mensagem de erro do tipo "A aplicação está a reiniciar", actualize a página **Administração Global**, no Microsoft Internet Explorer. |

Também pode instalar o RMS a partir de uma linha de comandos. Para mais instruções, consulte "[Instalação do Servidor do RMS a partir da Linha de Comandos](https://technet.microsoft.com/b55b1e2a-dd14-4168-a37f-9cdedbec660b)" posteriormente nesta secção.
