---
TOCTitle: Certificados de Licenciador de Clientes
Title: Certificados de Licenciador de Clientes
ms:assetid: 'bfb36387-3e15-4cde-8b8f-482219569a64'
ms:contentKeyID: 18124163
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747744(v=WS.10)'
---

Certificados de Licenciador de Clientes
=======================================

Um certificado de licenciador de clientes concede permissão a um autor para publicar conteúdo protegido pelo RMS sem estar ligado à rede da empresa.

Para obter um certificado de licenciador de clientes, um autor inicia um pedido de inscrição de cliente ao servidor de certificações de raiz ou a um servidor de licenciamentos de um computador cliente. O servidor devolve, então, um certificado de licenciador de clientes para esse computador.

Um certificado de licenciador de clientes contém a chave pública do licenciador de clientes, juntamente com a chave privada do licenciador de clientes que está encriptada pela chave pública do autor que pediu o certificado. Contém, também, a chave pública do servidor que emitiu o certificado, o qual está assinado pela chave privada do servidor que emitiu o certificado. A chave privada do licenciador de clientes é utilizada para assinar as licenças de publicação que o autor criar.
