---
TOCTitle: Definir as Permissões do Directório Virtual
Title: Definir as Permissões do Directório Virtual
ms:assetid: '45112111-9608-45b1-9a86-7b313d0a1579'
ms:contentKeyID: 18124000
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747549(v=WS.10)'
---

Definir as Permissões do Directório Virtual
===========================================

Após a activação da desactivação, esta fica disponível como um serviço. No entanto, o serviço de desactivação é um directório virtual do IIS com permissões de acesso associadas. Para que os utilizadores possam utilizar o serviço, tem de definir permissões no directório e no ficheiro real, decommission.asmx.

Por predefinição, a Autenticação Integrada do Windows foi activada para o directório virtual. No entanto, apenas as contas do sistema e do administrador têm acesso ao ficheiro real. Quando especifica as permissões para a DACL do ficheiro decommission.asmx, pode conceder acesso a um grupo de utilizadores específico para remover a protecção real do RMS ou pode conceder acesso ao serviço a todos os utilizadores.

Antes de os utilizadores poderem começar a utilizar o serviço de desactivação, a respectiva aplicação tem de ser modificada para que os pedidos de licença de utilização possam ser enviados para este novo pipeline de desactivação. Para o Microsoft Office System 2003, isto é efectuado através da adição de uma entrada de registo no computador do utilizador. Se estiver a utilizar o Office 2003, o procedimento a seguir pode ser utilizado para executar este passo:

1.  Abra o Editor de Registo.
2.  Navegue para `HKEY_CURRENT_USER\Software\Microsoft\Office\11.0\Common\DRM` e adicione uma chave nova chamada `Desactivação`.
3.  Na chave Desactivação, adicione a seguinte entrada nova de **Valor da Cadeia**, substituindo *servidor de licenças* pelo nome do servidor do RMS:
    `http://`*servidor de licenças*`/_wmcs/licensing`
4.  Em seguida, clique com o botão direito do rato na entrada e seleccione **Modificar** para especificar os dados de valor para apontar para o serviço de desactivação:
    `http://`*servidor de licenças*`/_wmcs/decommission`

| ![](/security-updates/images/Cc747549.note(WS.10).gif)Nota                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------|
| Podem existir diversas entradas para esta chave quando existem diversos servidores do RMS em modo de desactivação na organização. |
