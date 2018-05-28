---
TOCTitle: Para Excluir Certificados de Contas
Title: Para Excluir Certificados de Contas
ms:assetid: 'e5cd9dec-ac29-437e-8515-dc697ec75edf'
ms:contentKeyID: 18124203
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747785(v=WS.10)'
---

Para Excluir Certificados de Contas
===================================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

Estas condições são impostas pelo cliente na altura em que a licença de utilização está associada ao conteúdo protegido.

Excluir Certificados de Conta
-----------------------------

#### Para Excluir Certificados de Contas

1.  Abra a página **Administração Global** e, em seguida, no Web site em que pretende excluir certificados de contas, clique em **Administrar o RMS neste Web site**.

2.  Na área **Ligações da administração**, clique em **Políticas de exclusão**.

3.  Na área de exclusão do certificado e conta cliente em **Activar** para excluir um certificado de conta de direitos de um utilizador.

4.  Seleccione o método para especificar o certificado de conta a ser excluído:

    -   Para excluir certificados de contas por nome de utilizador, clique em **Nome de utilizador** para o certificado de conta a excluir, escreva o nome do utilizador a ser excluído (sob a forma *nome\_utilizador*@*nome\_domínio.com*) e, em seguida, clique em **Adicionar**. Utilize esta opção para excluir os certificados de contas de utilizadores internos que têm contas de utilizador do Active Directory.
    -   Para excluir um certificado de conta pela respectiva chave pública, clique em **Cadeia da chave pública** para o certificado de conta a excluir, escreva a respectiva cadeia da chave pública do certificado de conta e, em seguida, clique em **Adicionar**. Utilize esta opção para excluir os certificados de contas de utilizadores externos que não têm contas de utilizador do Active Directory.

    | ![](/security-updates/images/Cc747785.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                             |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Para eliminar um certificado de conta da lista de exclusões, clique no certificado de conta excluído na lista e, em seguida, clique em **Eliminar as chaves públicas seleccionadas da lista de exclusões**. O utilizador que possui esse certificado de conta poderá, então, obter uma licença para utilizar conteúdo protegido pelo RMS a partir deste servidor. |

    | ![](/security-updates/images/Cc747785.note(WS.10).gif)Nota                       |
    |---------------------------------------------------------------------------------------------|
    | Para desactivar a exclusão de certificados de contas de direitos, clique em **Desactivar**. |

Para mais informações sobre a execução deste procedimento, consulte "[Excluir Certificados de Conta](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)" anteriormente nesta secção.
