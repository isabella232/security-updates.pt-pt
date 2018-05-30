---
TOCTitle: Para Alterar as Definições de Proxy do RMS
Title: Para Alterar as Definições de Proxy do RMS
ms:assetid: '8f50bd4d-26b1-4996-b361-722ee21607f3'
ms:contentKeyID: 18124148
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747594(v=WS.10)'
---

Para Alterar as Definições de Proxy do RMS
==========================================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para mais informações acerca dos métodos de autenticação do servidor proxy e como funcionam no Windows Server 2003, consulte a ajuda dos Serviços de Informação Internet.

Alterar as Definições de Proxy do RMS
-------------------------------------

#### Para Alterar as Definições de Proxy do RMS

1.  Abra a página **Administração Global** e, em seguida, clique na ligação **Administrar o RMS neste Web site**.

2.  Em **Administração de cluster**, clique em **Definições de segurança**.

3.  Se não tiver utilizado um servidor proxy com o RMS anteriormente, seleccione a caixa de verificação **Este computador utiliza um servidor proxy para se ligar à Internet**. Serão apresentadas na página definições adicionais que deverá preencher.

4.  Na caixa **Endereço**, introduza o endereço IP ou nome de DNS do servidor proxy que pretende utilizar.

5.  Na caixa **Porta**, indique o número da porta que o servidor proxy utiliza para ligar à Internet.

6.  Se não utilizar o servidor proxy para se ligar aos recursos locais, seleccione a caixa de verificação **Ignorar servidor proxy para endereços locais**.

7.  Se necessário, seleccione a caixa de verificação **Este servidor proxy necessita de autenticação**.

    -   Seleccione o tipo de autenticação na lista: **Básica**, **Condensada** ou **Integrada do Windows**.
    -   Em **Nome de utilizador**, escreva o nome de utilizador que deve ser fornecido em resposta aos pedidos do servidor proxy.
    -   Em **Palavra-passe**, escreva a palavra-passe que deve ser fornecida em resposta aos pedidos do servidor proxy.
    -   Em **Confirmar a palavra-passe**, reintroduza a palavra-passe que especificou anteriormente, para verificar se a introduziu correctamente.
    -   Se o servidor proxy utilizar a autenticação integrada do Windows, em **Domínio**, indique o domínio a que pertence o utilizador.

8.  Clique em **Submeter**.
