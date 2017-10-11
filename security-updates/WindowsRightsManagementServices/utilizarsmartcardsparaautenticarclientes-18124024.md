---
TOCTitle: Utilizar Smart Cards para Autenticar Clientes
Title: Utilizar Smart Cards para Autenticar Clientes
ms:assetid: '5caacd67-fb16-46f1-b1ad-4aef0a632bf0'
ms:contentKeyID: 18124024
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747579(v=WS.10)'
---

Utilizar Smart Cards para Autenticar Clientes
=============================================

Se estiver a utilizar smart cards na organização para fornecer segurança e controlo adicionais para as credenciais de utilizador, pode agora utilizar esses smart cards quando obtiver certificados de contas de direitos e licenças de utilização a partir do servidor do RMS. Para configurar o servidor do RMS para requerer a autenticação do cliente, necessita de activar o Secure Sockets Layer (SSL) para o Web site no qual aprovisionou o RMS e configurar o método de autenticação nos Serviços de Informação Internet (IIS). Pode utilizar os seguintes passos para efectuar esta tarefa:

1.  Abra o **Gestor de Serviços de Informação Internet**.
2.  Expanda o item do servidor, clique com o botão direito do rato na pasta do Web site e clique em **Propriedades**.
3.  Clique no separador **Segurança de Directórios** e, na área **Comunicações Seguras**, seleccione a caixa de verificação **Activar o Mapeador do Serviço de Directório do Windows**.
4.  Expanda a pasta do Web site, abra o directório virtual **\_wmcs** e, em seguida, expanda o directório virtual (**Licencing** ou **Certification**) para o qual pretende configurar a autenticação.
    -   Para configurar a autenticação quando um utilizador pede uma licença de utilização, clique com o botão direito do rato no ficheiro license.asmx e clique em **Propriedades**.
    -   Para configurar a autenticação quando um utilizador pede um certificado de utilizador, clique com o botão direito do rato no ficheiro certification.asmx e clique em **Propriedades**.
5.  Clique no separador **Segurança de Ficheiros** e, na área **Comunicações Seguras**, clique em **Editar** para abrir a caixa de diálogo **Comunicações Seguras**.
6.  Seleccione **Exigir Canal Seguro (SSL)** e, em seguida, clique em:
    -   **Requerer Certificados de Cliente** se pretender que apenas os clientes com certificados do lado do cliente, tais como smart cards, sejam capazes de efectuar a ligação ao serviço.
    -   **Aceitar Certificados de Cliente** se pretender que os clientes tenham a opção de fornecer credenciais de autenticação com um certificado de smart card ou um nome de utilizador e uma palavra-passe.
7.  Seleccione **Activar Mapeamento de Certificados de Cliente** e, em seguida, clique em **OK**.
8.  Se pretender utilizar a autenticação de cliente para a certificação e para o licenciamento, repita este procedimento, seleccionando o directório virtual alternativo na segunda vez.

Depois de configurar estas definições, um utilizador que tente abrir conteúdo protegido pelo RMS e publicado por este servidor deverá fornecer credenciais de autenticação antes de o servidor fornecer um certificado de conta de direitos ou uma licença de utilização ao utilizador.
