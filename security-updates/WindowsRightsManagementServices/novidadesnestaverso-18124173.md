---
TOCTitle: Novidades nesta Versão
Title: Novidades nesta Versão
ms:assetid: 'c68ec6fd-0ff5-467e-85a8-a53b9f089de3'
ms:contentKeyID: 18124173
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747748(v=WS.10)'
---

Novidades nesta Versão
======================

Os Serviços de Gestão de Direitos (RMS) com Service Pack 1 (SP1) fornecem suporte para as seguintes funcionalidades:

-   **Inscrever o servidor do RMS sem ligação à Internet do servidor**. Na versão anterior, o servidor do RMS necessitava de se ligar à Internet para se inscrever no Serviço de Inscrição da Microsoft e receber o certificado de licenciador de servidores de raiz. Com o RMS SP1, o certificado de licenciador de servidores de raiz deve continuar a ser pedido a partir do Serviço de Inscrição da Microsoft, mas o pedido pode ser efectuado através de outro computador com ligação à Internet e, em seguida, importado para o servidor do RMS após o aprovisionamento.
-   **Clientes com activação automática**. Na versão anterior, os certificados de computadores e os cofres para os computadores clientes tinham de ser transferidos a partir do Serviço de Activação da Microsoft. Com o RMS SP1, não é necessário existir uma ligação com o Serviço de Activação da Microsoft.
-   **Suporte para mais tipos de clientes**. Nesta versão, o servidor do RMS pode ser utilizado para suportar clientes em dispositivos móveis e serviços de servidor. Na qualidade de administrador do servidor do RMS, pode controlar se o servidor fornece ou não certificação para estes clientes quando estes tentam utilizar os serviços.
-   **Suporte para múltiplos modelos de idioma**. Na versão anterior, os modelos baseavam-se na definição de idioma do Internet Explorer. Nesta versão, pode utilizar a página Web Administração do RMS para especificar o idioma a utilizar na criação de um modelo.
-   **Suporte para autenticação de clientes com smart cards**. Nesta versão, o cliente do RMS pode utilizar credenciais armazenadas como certificados x.509 em smart cards para efectuar a autenticação junto do servidor do RMS e obter certificados de contas de direitos (RACs) e licenças de utilização.
