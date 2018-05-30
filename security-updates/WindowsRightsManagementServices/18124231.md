---
TOCTitle: Definir Políticas de Fidedignidade
Title: Definir Políticas de Fidedignidade
ms:assetid: 'e8d78300-4b26-4f15-9e4f-5ae9eb827ef9'
ms:contentKeyID: 18124231
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747711(v=WS.10)'
---

Definir Políticas de Fidedignidade
==================================

Pode definir os utilizadores e os domínios de publicação fidedignos da seguinte forma:

-   **Domínios de utilizadores fidedignos**. Quando adicionar um domínio de utilizadores, o RMS poderá processar pedidos de licenças de utilização de utilizadores cujos certificados de contas de direitos foram emitidos por uma instalação do RMS existente numa outra floresta do Active Directory; por outras palavras, um cluster de certificações de raiz diferente. Pode adicionar um domínio de utilizadores fidedignos através da importação do certificado de licenciador de servidores da instalação a ser considerada fidedigna.
-   **Domínios de publicação fidedignos**. A adição de um domínio de publicação permite a um servidor do RMS emitir licenças de utilização referentes às licenças de publicação emitidas por um outro servidor do RMS. Pode adicionar um domínio de publicação fidedigno através da importação do certificado de licenciador de servidores e da chave privada do servidor a ser considerado fidedigno.

Para mais informações, consulte "[Adicionar e Remover Domínios de Utilizadores Fidedignos](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)" e "[Adicionar e Remover Domínios de Publicação Fidedignos](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee)" posteriormente nesta secção. Para obter instruções detalhadas, consulte "[Estabelecer Políticas de Fidedignidade](https://technet.microsoft.com/6c2be3c2-1837-4de4-a72e-3ba3eec3321d)" posteriormente nesta secção.
