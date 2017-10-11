---
TOCTitle: Certificados de Conta de Direitos
Title: Certificados de Conta de Direitos
ms:assetid: '2ff315cc-211d-4e6e-85e8-56867c2abd94'
ms:contentKeyID: 18123922
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720230(v=WS.10)'
---

Certificados de Conta de Direitos
=================================

As organizações têm de identificar os utilizadores que são considerados entidades fidedignas no respectivo sistema do RMS. Para tal, o RMS emite certificados de contas de direitos que associam as contas de utilizadores a computadores específicos. O certificado de conta de direitos do utilizador tem de ser incluído no pedido de certificados de licenciador de clientes e de licenças de utilização. Um certificado de licenciador de clientes permite a um autor publicar conteúdo protegido pelo RMS, tal como ficheiros e mensagens de correio electrónico, quando está offline. Uma licença de utilização permite a um utilizador consumir conteúdo protegido pelo RMS. Cada certificado de conta de direitos contém a chave pública do utilizador que é utilizada na encriptação dos dados destinados a esse utilizador.

Existem dois tipos de certificados de contas de direitos: padrão e temporário. Pode especificar um período de validade para ambos os tipos. Os certificados padrão têm uma duração especificada em dias (por predefinição, 365 dias). Os certificados de contas temporários têm uma duração especificada em minutos (por predefinição, 15 minutos). Os certificados de contas temporários permitem aos utilizadores consumir conteúdo temporariamente, por exemplo num quiosque, quando não conseguem aceder ao computador que geralmente costumam utilizar. Isto impede que, posteriormente, outro utilizador possa vir a consumir esse conteúdo do mesmo computador.
