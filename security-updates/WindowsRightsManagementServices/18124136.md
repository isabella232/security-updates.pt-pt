---
TOCTitle: Domínios de Publicação Fidedignos
Title: Domínios de Publicação Fidedignos
ms:assetid: 'bca1c33a-d3ef-42b5-adbe-6e104979a71f'
ms:contentKeyID: 18124136
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747738(v=WS.10)'
---

Domínios de Publicação Fidedignos
=================================

Por predefinição, os servidores do RMS não emitem licenças de utilização para licenças de publicação emitidas por um servidor do RMS existente num cluster diferente. Existem situações, contudo, em que o mesmo servidor ou cluster não pode emitir licenças de publicação e de utilização para uma peça de conteúdo protegido. Isto pode ocorrer quando um cluster específico do RMS é removido e substituído. Por exemplo, em caso de fusão de duas empresas. Nesta situação, um cluster do RMS necessita de poder emitir licenças de utilização para licenças de publicação criadas por um cluster diferente do RMS.

Pode configurar um cluster do RMS para confiar nas licenças de publicação emitidas por um cluster diferente do RMS e emitir licenças de utilização através da implementação de um domínio de publicação fidedigno. Para isso, importe o certificado de licenciador de servidores e a chave privada do outro servidor e, em seguida, adicione-os à lista de domínios de publicação fidedignos. As chaves privadas que são importadas são utilizadas apenas para desencriptar licenças de publicação assinadas, e não para assinar novas licenças.

Para mais informações sobre domínios de utilizadores fidedignos e obter instruções detalhadas, consulte "Adicionar e Remover Domínios de Publicação Fidedignos" e "Estabelecer Políticas de Fidedignidade" em "Utilizar um Servidor do RMS" nesta colecção de documentação.
