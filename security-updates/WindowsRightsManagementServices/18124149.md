---
TOCTitle: Problemas de Aprovisionamento do RMS
Title: Problemas de Aprovisionamento do RMS
ms:assetid: 'b0e6ef48-ab38-4426-be5b-811cf64c45c0'
ms:contentKeyID: 18124149
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747638(v=WS.10)'
---

Problemas de Aprovisionamento do RMS
====================================

Quando aprovisionar o RMS, os ficheiros dos recursos e as ligações entre os vários componentes do RMS são configurados e estabelecidos. Se for detectado um erro enquanto o RMS estiver a tentar configurar um recurso, o aprovisionamento falha e aparece uma mensagem de erro. Esta secção analisa as causas mais comuns destes erros para o ajudar a resolver situações inesperadas que impeçam a conclusão do aprovisionamento do RMS.

Não é Possível Aprovisionar o Servidor de Certificações de Raiz
---------------------------------------------------------------

Poderá não ser possível aprovisionar um servidor de certificações de raiz porque não aparecem as páginas de aprovisionamento correctas. Este comportamento pode ocorrer quando clicar em Aprovisionar o RMS neste Web site para aprovisionar o primeiro servidor de certificações de raiz da página Administração Global. No entanto, em vez de aprovisionar as páginas para um servidor de certificações de raiz, aparecem as páginas para aprovisionar um servidor de licenciamento.

Este problema ocorre quando não desaprovisionar o último servidor de certificações de raiz nesta floresta do Active Directory antes de desinstalar o RMS da floresta e, em seguida, tentar aprovisionar um servidor de certificações de raiz. Quando desaprovisionar o único servidor de certificações de raiz que está na floresta do Active Directory, remove o ponto de ligação do serviço do Active Directory. Se não desaprovisionar o último servidor de certificações de raiz que está na floresta antes de desinstalar o RMS, não conseguirá aprovisionar novamente um servidor de certificações de raiz que está na floresta antes de remover manualmente o ponto de ligação do serviço do Active Directory.

Se as páginas de aprovisionamento de um servidor de licenciamento aparecerem quando tentar aprovisionar o primeiro servidor de certificações de raiz numa floresta do Active Directory, remova o ponto de ligação do serviço a partir do Active Directory da seguinte forma:

**Para remover o ponto de ligação do serviço do RMS**
1.  Se for necessário, instale as Ferramentas de Suporte do Windows Server:

    Para o Windows Server 2003, a partir da pasta \\Support\\Tools que se encontra no CD de instalação, execute Suptools.msi.

    Para o Windows 2000 Server, a partir da pasta \\Support Tools que se encontra no CD de instalação, execute o Setup.exe.

2.  Inicie a sessão no controlador do domínio em que o servidor de certificações de raiz é membro utilizando uma conta de um membro do grupo Admins do Domínio.

3.  Na linha de comandos, escreva o seguinte comando e, em seguida, prima ENTER:

    **ldp**

4.  Clique em **Ligação** e, em seguida, em **Ligar**.

5.  Prima ENTER. Não escreva mais nenhuma informação.

6.  Clique em **Ligação** e, em seguida, em **Juntar**.

7.  Prima ENTER. Não escreva mais nenhuma informação.

8.  Clique em **Ver** e, em seguida, em **Árvore**.

9.  Prima ENTER. Não escreva mais nenhuma informação.

    **dc=SeuDomínio,dc=com** é apresentado no painel da esquerda.

10. Expanda **dc= SeuDomínio,dc=com**.

11. Expanda **Configuração**.

12. Expanda **Serviços**.

13. Elimine **RightsManagementServices**.

- ou -

1.  Transfira e instale o Kit de Ferramentas de Administração do RMS. O kit de ferramentas pode ser transferido a partir do [Web site da Microsoft](http://go.microsoft.com/fwlink/?linkid=33841).
2.  Abra a Linha de comandos, clicando em **Iniciar**, **Executar**. Na caixa de diálogo **Executar**, escreva **cmd** e, em seguida, clique em **OK**.
3.  Na linha de comandos, escreva o seguinte comando:
    **ADSCPRegister.exeunregisterscp** &lt;*URLtoUnRegister*&gt;
4.  Para &lt;*URLtoUnRegister*&gt;, escreva o URL desse ponto de ligação do serviço do RMS, por exemplo, https://my\_domain/\_wmcs/Certification.

Depois de concluir estes passos, pode aprovisionar o servidor de certificações de raiz.

Não é Possível Gerar o Contexto SSPI
------------------------------------

Pode receber uma mensagem de erro "Não é possível gerar o contexto SSPI" durante o aprovisionamento se a conta de serviço do RMS não for autenticada quando inscrever o servidor de certificações de raiz com o Serviço de Inscrição da Microsoft.

Se receber esta mensagem de erro, deve verificar se a conta de serviço do RMS é uma conta de domínio válida. Se a conta for uma conta de grupo, verifique se os membros do grupos são actuais, se pode resolver todas as contas de utilizadores no grupo do domínio e se as contas têm permissões para as bases de dados SQL.
