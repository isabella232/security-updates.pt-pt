---
TOCTitle: Para Excluir Aplicações
Title: Para Excluir Aplicações
ms:assetid: '422f2ddd-bcf4-45f1-905a-b8bad30fd7dd'
ms:contentKeyID: 18123958
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720262(v=WS.10)'
---

Para Excluir Aplicações
=======================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

As políticas de exclusão são impostas pelo cliente na altura em que a licença de utilização está associada ao conteúdo protegido.

Excluir Aplicações ou Parar a Exclusão de Aplicações
----------------------------------------------------

#### Para Excluir Aplicações

1.  Abra a página **Administração Global** e, em seguida, no Web site em que pretende controlar as versões das aplicações que podem ser utilizadas com o conteúdo protegido pelos direitos, clique em **Administrar o RMS neste Web site**.

2.  Na área de **ligaçõesAdministração**, clique em **Políticas de exclusão**.

3.  Na área **Exclusão da aplicação**, clique em **Activar**, para excluir uma aplicação ou um componente activado pelo RMS.

    Para desactivar a exclusão da aplicação, clique em **Desactivar**.

4.  Escreva o nome do ficheiro da aplicação ou do componente a ser excluído, escreva as versões mínima e máxima a serem excluídas (no formato *x*.*x*.*x*.*x*) e, em seguida, clique em **Excluir esta aplicação**.

    Para eliminar uma aplicação (ou componente) da lista de exclusões, seleccione o nome do ficheiro e, em seguida, clique em **Eliminar as aplicações seleccionadas da lista de exclusões**.

    | ![](/security-updates/images/Cc720262.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                    |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | O RMS requer que especifique a versão da aplicação num formato de 4 dígitos delimitados por pontos (\#.\#.\#.\# ). No entanto, algumas aplicações especificam a respectiva versão através de um número de 2 ou 3 dígitos delimitado por pontos. Neste caso, deverá adicionar um .0 conforme adequado para corresponder o número da versão ao formato requerido pelo RMS. |

#### Para Parar a Exclusão de Aplicações

1.  Abra a página **Administração Global** e, em seguida, no Web site em que pretende controlar as versões das aplicações que podem ser utilizadas com o conteúdo protegido pelos direitos, clique em **Administrar o RMS neste Web site**.

2.  Na área de **ligaçõesAdministração**, clique em **Políticas de exclusão**.

3.  Na área **Exclusão da aplicação**, clique em **Desactivar**.

Para mais informações sobre a execução deste procedimento, consulte "[Excluir Aplicações](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)" anteriormente nesta secção.
