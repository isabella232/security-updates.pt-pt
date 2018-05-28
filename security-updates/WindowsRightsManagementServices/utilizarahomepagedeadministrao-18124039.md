---
TOCTitle: Utilizar a Home Page de Administração
Title: Utilizar a Home Page de Administração
ms:assetid: '6c155977-bd0e-47d6-ac65-1746cddb505e'
ms:contentKeyID: 18124039
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720290(v=WS.10)'
---

Utilizar a Home Page de Administração
=====================================

A partir da página Web **Administração**, pode ver informações sobre o servidor ou o cluster e aceder às opções de administração. Esta página só está disponível depois de o servidor ter sido aprovisionado.

Para aceder a esta página Web a partir do servidor que pretende administrar, utilize os seguintes passos:

1.  Inicie a sessão como administrador local.
2.  Clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e seleccione **Administração do Windows RMS**.
3.  Na página **Administração Global**, clique em **Administrar o RMS neste Web site**.

Se activou a administração remota utilizando o Secure Sockets Layer (SSL), pode também aceder à **Home page de Administração** a partir de um computador diferente, se executar os seguintes passos:

1.  Na barra de endereços do seu browser, escreva o seguinte URL:
    https://*nome\_do\_cluster:número\_da\_porta*/\_wmcs/admin
    No qual *nome\_do\_cluster:número\_da\_porta* é o URL que especificou para este cluster durante o aprovisionamento. Escreva o número da porta apenas no caso de ter especificado um número que não é o número de porta predefinido (80).
2.  Quando lhe for indicado, escreva as credenciais de um administrador local no servidor que está a aceder.

A **Home page de Administração** apresenta informações sobre o cluster, tais como o URL do cluster, nome e localização da base de dados de configuração, data de expiração do certificado de licenciador de servidores, etc. Proporciona também ligações a páginas onde pode configurar as seguintes opções de administração do cluster:

-   **Políticas de fidedignidade.** Adicione e remova domínios fidedignos. Para mais informações, consulte "[Gerir a Confiança e a Política de Fidedignidade](https://technet.microsoft.com/1c96ee74-fd28-4511-be21-087e2b04c3ee)" posteriormente nesta secção.
-   **Modelos de política de direitos**. Criar e modificar modelos de política de direitos. Para mais informações, consulte "[Gerir Modelos de Política de Direitos.](https://technet.microsoft.com/718286dc-3399-4556-96c9-ec3a33d31877)" posteriormente nesta secção.
-   **Definições de registo**. Activar e desactivar o registo e ver o nome do servidor de registo e da base de dados. Para mais informações, consulte "[Gerir o Registo](https://technet.microsoft.com/8fccfc57-2135-494e-8e44-f6191bf5e4a0)" posteriormente nesta secção.
-   **Definições do URL do cluster da extranet.** Especifique um URL externo disponível para os pedidos de licenciamento e certificação de contas. Para mais informações, consulte "[Configurar o URL de uma Extranet](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)" posteriormente nesta secção.
-   **Definições de proxy do RMS.** Especifique o endereço do servidor proxy, o tipo de autenticação e o nome de utilizador a ser utilizado quando o servidor de RMS necessitar de estabelecer uma ligação à Internet através de um servidor proxy. Para mais informações, consulte "[Configurar as Definições de Proxy do RMS](https://technet.microsoft.com/179d2970-62e9-4487-aa5b-f4334234991e)" posteriormente nesta secção.
-   **Definições de segurança.** Reponha a palavra-passe da chave privada do servidor, especifique o grupo de super utilizadores cujos membros podem desencriptar todo o conteúdo licenciado e desactive o RMS. Para mais informações, consulte "[Gerir a Segurança Durante a Utilização do RMS](https://technet.microsoft.com/62050812-de4f-4392-8d63-f2f89aa01ed4)" posteriormente nesta secção.
-   **Definições de certificação.** Especifique o período de validade dos certificados de contas de direitos e especifique um contacto administrativo. (Esta opção está disponível apenas no cluster de certificações de raiz, e não nos servidores de licenciamentos.) Para mais informações, consulte "[Gerir Certificados de Conta](https://technet.microsoft.com/49c5c2ba-e197-4e4b-b3b3-b3248f068bcc)" posteriormente nesta secção.
-   **Políticas de exclusão.** Especifique a exclusão com base na versão do cofre, no certificado de contas de direitos, na versão do Windows ou numa aplicação activada pelo RMS. Para mais informações, consulte "[Gerir a Política de Exclusão](https://technet.microsoft.com/ee31e099-e095-4648-95da-0009fbeb48cb)" posteriormente nesta secção.
-   **Relatório de certificação de contas de gestão de direitos (RM).** Veja o número de certificados de contas que foram emitidos. (Esta opção está disponível apenas no cluster de certificações de raiz, e não nos servidores de licenciamentos.) Para mais informações, consulte "[Rastrear Certificados de Conta](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)" posteriormente nesta secção.

Os restantes tópicos incluídos nesta secção descrevem a forma como estas funcionalidades podem ser utilizadas. Para obter instruções detalhadas, consulte “[RMS - Como ...](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)” posteriormente nesta secção.

| ![](/security-updates/images/Cc720290.note(WS.10).gif)Nota                                                                                                                                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| O Web site da Administração do RMS utiliza janelas de contexto para a configuração de algumas funcionalidades. Se estiver a utilizar um bloqueador de contexto no seu browser Web, deverá configurar as definições do browser para permitir que apareçam janelas de contexto do Web site da Administração do RMS. |
