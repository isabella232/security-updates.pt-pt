---
TOCTitle: Para Considerar Fidedignos os Certificados de Contas Baseados no Passport
Title: Para Considerar Fidedignos os Certificados de Contas Baseados no Passport
ms:assetid: 'c096fa36-c40d-4b28-843c-e9cbbe8eef70'
ms:contentKeyID: 18124145
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747655(v=WS.10)'
---

Para Considerar Fidedignos os Certificados de Contas Baseados no Passport
=========================================================================

A Microsoft fornece um serviço de certificação de contas que utiliza as credenciais do Microsoft .NET Passport para estabelecer o certificado de conta de direitos para o utilizador. Se pretender que os utilizadores com os certificados de conta de direitos desse serviço possam obter licenças de utilização a partir do seu cluster do RMS, deve configurar um domínio de utilizadores fidedignos que aceite credenciais de utilizador do serviço de certificação de contas da Microsoft.

Para utilizar esta funcionalidade, deve configurar os Serviços de Informação Internet para permitir o acesso anónimo ao serviço de licenciamento do RMS. Este passo é essencial para os utilizadores externos, uma vez que o serviço de licenciamento está configurado para utilizar por predefinição a Autenticação Integrada do Windows. Se o acesso anónimo não estiver definido, os utilizadores externos com Certificados de Contas de Direitos (RACs) baseados no Passport não poderão obter licenças.

Considerar Fidedignos os Certificados de Contas Baseados no Passport
--------------------------------------------------------------------

#### Para permitir o acesso anónimo ao serviço de licenciamento do RMS

1.  Abra o snap-in **Gestor de Serviços de Informação Internet (IIS)** e expanda o servidor que está a alojar o RMS.

2.  Na árvore da consola, expanda **Web sites** e expanda o Web site em que configurou o RMS. Por predefinição, é o **Web site Predefinido**.

3.  Na árvore da consola, expanda o Web site **\_wmcs** e seleccione o directório virtual para **licenciamento**.

4.  Clique com o botão direito no directório virtual para **licenciamento** e seleccione **Propriedades**.

5.  Na caixa de diálogo de **Propriedades de Licenciamento**, clique no separador de **segurança de directório**.

6.  Clique em **Editar** na área de **Autenticação e controlo de acesso**.

7.  Seleccione a caixa de verificação para **Permitir Acesso Anónimo**.

#### Para Considerar Fidedignos os Certificados de Contas Baseados no Passport

1.  Abra a página **Administração Global** e, em seguida, no Web site em que pretende considerar fidedignos os certificados de contas baseados no Passport, clique em **Administrar o RMS neste Web site**.

2.  Na área **Ligações da administração**, clique em **Políticas de fidedignidade**.

3.  Na área **Domínios de utilizadores fidedignos**, clique em **Considerar fidedignos todos os RACs do Passport**. O Microsoft RM Certification Service aparece na lista **Domínios de utilizadores fidedignos**.

4.  Opcionalmente, pode excluir utilizadores com base nos respectivos endereços de correio electrónico. Para isso, clique em **Identidades excluídas** e, em seguida, escreva o endereço de correio electrónico do utilizador que não é considerado fidedigno.
