---
TOCTitle: 'Passo 2: Instalar o WSUS 3.0 no Servidor'
Title: 'Passo 2: Instalar o WSUS 3.0 no Servidor'
ms:assetid: '191e62a0-7671-41eb-9841-17c64313fa68'
ms:contentKeyID: 18141980
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720469(v=WS.10)'
---

Passo 2: Instalar o WSUS 3.0 no Servidor
========================================

Depois de assegurar que o servidor preenche os requisitos de instalação, está preparado para instalar o WSUS 3.0. Terá de iniciar sessão no servidor no qual pretende instalar o WSUS 3.0 utilizando uma conta membro do grupo Administradores local. Apenas os membros do grupo Administradores local podem instalar o WSUS 3.0.

O seguinte procedimento utiliza as opções de instalação do WSUS predefinidas, que incluem a instalação do Base de dados interna do Windows para o software de base de dados do WSUS 3.0, o armazenamento local das actualizações e a utilização do Web site predefinido do IIS na porta 80.

**Para instalar o WSUS 3.0**
1.  Faça duplo clique no ficheiro de instalação, **WSUSSetup.exe**.

2.  Na página **Bem-vindo** do assistente de instalação, clique em **Seguinte**.

3.  Na página **Selecção do Modo de Instalação**, clique em **Instalação completa de servidor incluindo Consola de Administração**, se quiser instalar o servidor neste computador, ou em **Apenas Consola de Administração**, se quiser instalar apenas a consola de administração.

4.  Na página **Contrato de Licença**, leia atentamente os termos do contrato de licença, clique em **Aceito os termos do Contrato de Licença** e, depois, clique em **Seguinte**.

    ![](images/Cc720469.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Na página **Seleccionar Origem de Actualização** do assistente de instalação, pode especificar de onde os clientes deverão obter actualizações. Se seleccionar a caixa de verificação **Armazenar actualizações localmente**, as actualizações são armazenadas no servidor com o WSUS 3.0, sendo necessário seleccionar uma localização no sistema de ficheiros para armazenamento das actualizações. Se as actualizações não forem armazenadas localmente, os computadores cliente irão ligar ao Microsoft Update para obter actualizações aprovadas. Mantenha as opções predefinidas e clique em **Seguinte**.

    ![](images/Cc720469.c8bac396-ca39-4491-8b0c-742a0e470535(WS.10).gif)

6.  Na página **Opções de Base de Dados**, seleccione o software utilizado para gerir a base de dados do WSUS 3.0. Por predefinição, a Configuração do WSUS dá-lhe a possibilidade de instalar o Base de dados interna do Windows, caso o computador onde está a efectuar a instalação tenha o Windows Server 2003.

7.  Se não quiser utilizar o Base de dados interna do Windows, terá de fornecer uma instância SQL Server que o WSUS possa utilizar. Para tal, clique em **Utilizar** **um servidor de base de dados existente neste computador** e escreva o nome da instância na caixa. O nome da instância deverá aparecer como &lt;*serverName*&gt;\\&lt;*instanceName*&gt;, em que *serverName* é o nome do servidor e *instanceName* é o nome da instância de SQL. Faça a sua selecção e, depois, clique em **Seguinte**.

8.  Na página **A ligar à instância de servidor de SQL**, o WSUS tenta estabelecer ligação à instância do SQL Server especificada. Quando tiver estabelecido ligação com êxito, clique em **Seguinte** para continuar.

    ![](images/Cc720469.36c6af0c-a61e-4151-ae50-c754a106cb1b(WS.10).gif)

9.  Na página **Selecção de Web Site**, especifique o Web site que o WSUS 3.0 irá utilizar. Se pretender utilizar o Web site predefinido do IIS na porta 80, seleccione a primeira opção. Se já tiver um Web site na porta 80, pode criar um site alternativo na porta 8530 seleccionando a segunda opção. Mantenha a opção predefinida e clique em **Seguinte**.

10. Na página **Pronto para instalar o Windows Server Update Services**, reveja as selecções e, depois, clique em **Seguinte**.

11. Na página final da instalação, o assistente irá indicar se a instalação do WSUS 3.0 foi ou não concluída com êxito. Depois de clicar em **Concluir**, é iniciado o assistente de configuração.
