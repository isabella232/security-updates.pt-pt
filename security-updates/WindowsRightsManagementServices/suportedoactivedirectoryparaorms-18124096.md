---
TOCTitle: Suporte do Active Directory para o RMS
Title: Suporte do Active Directory para o RMS
ms:assetid: '9589127d-19b3-44f1-b7a1-01992e78218a'
ms:contentKeyID: 18124096
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747604(v=WS.10)'
---

Suporte do Active Directory para o RMS
======================================

O RMS utiliza o Active Directory com os seguintes objectivos:

-   **Fornecer autenticação de utilizador.** O Active Directory fornece os serviços de directório utilizados na autenticação de utilizadores para o RMS. Para mais informações sobre a autenticação e o RMS, consulte "[Modelo de Segurança do RMS](https://technet.microsoft.com/665db831-366d-4dca-9bb3-cc2912481fe1)" posteriormente nesta secção.
-   **Resolver membros de grupo e identidades de conta de utilizador individuais.** O Active Directory fornece informações sobre os membros do grupo que o RMS utiliza para conceder licenças de utilização ao conteúdo protegido pelo RMS quando a licença de publicação concede direitos a grupos e não a contas de utilizador individuais. Para reduzir o número de consultas LDAP efectuadas no Active Directory, o RMS coloca em cache as informações obtidas numa cache local, armazenando-as também numa base de dados centralizada de serviços de directório. Para mais informações, consulte "[Cache do Active Directory do RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)" e "[Base de Dados de Serviços de Directório do RMS](https://technet.microsoft.com/6f6b8586-5d17-4a40-94a3-4dc738195301)" anteriormente nesta secção.
-   **Armazenar a localização de identificação do serviço do RMS.** Os pedidos de serviço (como os de uma licença de utilização, uma licença de publicação ou a pré-inscrição de um servidor de licenciamento) têm de ser enviados para o URL do módulo executável do serviço Web que está a conceder o pedido. Todos os pedidos de serviço começam por uma consulta ao Active Directory para determinar o URL do servidor do serviço Web (Server.asmx), o qual, por sua vez, fornece o URL apropriado para o pedido de serviço. Para mais informações, consulte "[Publicação e Identificação de Serviços do RMS](https://technet.microsoft.com/336c0d55-fd7f-4aa9-b3e6-bfd6565b1086)" posteriormente nesta secção.
