---
TOCTitle: Para Inscrever Manualmente um Servidor de certificações de Raiz
Title: Para Inscrever Manualmente um Servidor de certificações de Raiz
ms:assetid: 'aecdebb5-b28b-4b58-937a-392bb6ce9643'
ms:contentKeyID: 18124122
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747727(v=WS.10)'
---

Para Inscrever Manualmente um Servidor de certificações de Raiz
===============================================================

Para efectuar este procedimento necessita de ter iniciado a sessão localmente no Web site de Administração com uma conta de utilizador de domínio que seja membro do grupo de administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como procedimento de segurança recomendado, considere utilizar o comando Executar como para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

Se estiver a utilizar o processo de inscrição offline, certifique-se de que os clientes do RMS não tentam efectuar a ligação ao servidor RMS para licenças até terminar a inscrição. Se os clientes tentarem efectuar a ligação a um servidor RMS que não esteja inscrito, ocorre um erro nos serviços que os torna inúteis. Caso não consiga assegurar que os clientes não tentam efectuar a ligação ao servidor RMS, a melhor opção será repor o IIS depois de terminar a inscrição para limpar quaisquer erros que possam ter ocorrido.

Se seleccionou utilizar a inscrição offline e se estiver a utilizar um computador que tenha uma configuração de segurança do browser melhorada, como um computador com o Windows Server 2003 ou Windows XP Service Pack 2, para efectuar a ligação à Internet e pedir um certificado de licenciador de site servidores, certifique-se de que adiciona o URL do Web site do Serviço de Inscrição na zona de Sites Fidedignos para permitir a transferência do certificado de licenciador de servidores. Este URL é URL https://activation.drm.microsoft.com.

Se estiver a utilizar o processo de inscrição offline, certifique-se de que o computador que está a utilizar para submeter o pedido de inscrição ao Serviço de Inscrição da Microsoft Enrollment Service tem a CA GTE Cyber Trust Root instalada no armazenamento de certificados. Esta autoridade de certificação é considerada fidedigna por predefinição em máquina com o Windows Server 2003. Se o computador tiver outra versão do Windows, pode tornar fidedigna esta CA instalando as actualizações mais recentes do certificado a partir do Windows Update.

Inscrever Manualmente um Servidor de Certificações de Raiz
----------------------------------------------------------

#### Para Inscrever Manualmente um Servidor de Certificações de Raiz

1.  Depois de instalar o RMS num servidor que deseja que seja o servidor de certificação de raiz, abra a página **Administração Global** e, ao lado do Web site em que deseja importar um certificado de licenciador de servidores de raiz, clique em **Administrar o RMS neste Web site**.

2.  Na área **Recursos de cluster** clique em **Inscrever**. A caixa de diálogo **Inscrever** abre-se.

3.  Seleccione a opção **Offline** e clique no botão **Exportar**. Aparece a caixa de diálogo **Transferência de ficheiros**.

4.  Clique em **Guardar**. Aparece a caixa de diálogo **Guardar como**.

    | ![](/security-updates/images/Cc747727.note(WS.10).gif)Nota                                                                                                                |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Na caixa de diálogo **Transferência de Ficheiros**, não clique em **Abrir**. Se clicar em **Abrir** aparece uma mensagem de erro e o ficheiro de pedido de inscrição não é guardado. |

5.  Clique em **Guardar** para exportar o pedido de inscrição para um ficheiro. Por predefinição, o ficheiro é guardado no ambiente de trabalho e é-lhe atribuído o nome *Nome\_servidor*EnrollRequest.xml, em que *nome\_servidor* é substituído pelo nome do servidor do RMS. Pode guardar o ficheiro numa localização diferente seleccionando a localização que deseja a partir do menu pendente **Guardar em**. Também pode alterar o nome de ficheiro em **Nome de ficheiro**.

6.  Depois de guardar o ficheiro de pedido de inscrição, aparece a caixa de diálogo **Transferência concluída**. Pode clicar em **Abrir** para ver o código XML no ficheiro, mas não pode fazer alterações no ficheiro. Para abrir a pasta onde o ficheiro está armazenado, clique em **Abrir pasta**. Clique em **Fechar** se terminou a procura no ficheiro e a verificação da sua localização.

7.  Transfira o ficheiro de pedido de inscrição do servidor para um computador com ligação à Internet e, em seguida, navegue pelo Web site do [Serviço de Inscrição]().

8.  Siga as instruções no Web site para obter um certificado de licenciador de servidores.

9.  Volte a colocar o certificado de licenciador de servidores na certificação de raiz.

10. Na área **Recursos de cluster** clique em **Inscrever**. A caixa de dialogo **Inscrever** abre.

11. Na caixa de diálogo **Inscrever**, clique no botão **Procurar** e localize o certificado de licenciador de servidores que transferiu e, em seguida, clique no botão **Importar**.

12. Clique em **Sim** para confirmar que deseja importar este certificado.

13. A área **Recursos de cluster** é actualizada para exibir o certificado de licenciador de servidores.
