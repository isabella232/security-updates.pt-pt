---
TOCTitle: Adicionar e Remover Domínios de Utilizadores Fidedignos
Title: Adicionar e Remover Domínios de Utilizadores Fidedignos
ms:assetid: '7c440b15-01c4-49f1-b43c-00f67f3388c1'
ms:contentKeyID: 18124066
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747571(v=WS.10)'
---

Adicionar e Remover Domínios de Utilizadores Fidedignos
=======================================================

Por predefinição, o RMS não satisfaz os pedidos de utilizadores cujos certificados de contas de direitos foram emitidos por uma outra instalação do RMS. No entanto, pode adicionar domínios de utilizador à lista de domínios de utilizadores fidedignos, o que permite ao RMS processar esses pedidos.

Pode também adicionar e remover utilizadores ou grupos de utilizadores específicos em cada domínio fidedigno. Pode também remover um domínio de utilizadores fidedignos, mas não é possível remover o cluster de certificações de raiz dessa floresta do Active Directory dos domínios de utilizadores fidedignos. Todos os servidores do RMS de uma implementação, incluindo o servidor de certificações de raiz, confiam no cluster de certificações de raiz da sua própria floresta.

Pode gerir os domínios de utilizadores fidedignos da seguinte forma:

-   De um modo geral, pode adicionar o serviço Microsoft® .NET Passport à lista de domínios fidedignos para suportar os utilizadores externos. Isto permite a um servidor do RMS da sua empresa processar pedidos de licenciamento que incluam um certificado de conta de direitos emitido pelo Serviço Microsoft .NET Passport.
-   Para tornar fidedignos os utilizadores externos da instalação do RMS de outra organização, pode adicionar essa organização à lista de domínios de utilizadores fidedignos. Isto permite ao servidor do RMS processar um pedido de licenciamento que inclua um certificado de conta de direitos emitido por um servidor do RMS pertencente a outra organização.
-   Para processar pedidos de licenciamento de utilizadores da sua organização que pertençam a uma floresta diferente do Active Directory, pode adicionar a instalação do RMS dessa floresta à lista de domínios de utilizadores fidedignos. Isto permite ao servidor do RMS da floresta actual processar um pedido de licenciamento que inclua um certificado de conta de direitos emitido por um servidor do RMS pertencente a outra floresta.
-   Para cada domínio de utilizadores fidedignos, pode especificar os domínios de correio electrónico fidedignos. Para domínios Passport fidedignos, pode especificar os domínios ou os utilizadores de correio electrónico não fidedignos.

Para adicionar uma instalação do RMS à lista de domínios de utilizadores fidedignos, é necessário importar o certificado de licenciador de servidores para a instalação do RMS que pretende adicionar. O administrador deverá primeiro exportar o certificado de licenciador de servidores do servidor ou cluster fidedigno e enviar-lhe o ficheiro do certificado. Em seguida, pode importar o ficheiro, especificando a respectiva localização. Para guardar o ficheiro, o utilizador que iniciou a sessão deverá dispor de permissões para a pasta partilhada. As informações relativas à chave privada não são transferidas quando é configurado um domínio de utilizadores fidedignos.

Para obter instruções detalhadas para estabelecer domínios de utilizadores fidedignos, consulte "[Para Adicionar um Domínio de Utilizadores Fidedignos](https://technet.microsoft.com/ed672e58-6272-4ac0-a434-d1d938037e93)" posteriormente nesta secção.
