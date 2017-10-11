---
TOCTitle: Publicação Online
Title: Publicação Online
ms:assetid: '962c4e83-cf34-4c61-9589-31d24b0299fb'
ms:contentKeyID: 18124102
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747694(v=WS.10)'
---

Publicação Online
=================

O seguinte diagrama descreve o processo de publicação online.

![](images/Cc747694.897e47b6-fffe-4b11-bc9f-be58539b9f19(WS.10).gif)

O processo de publicação online envolve os seguintes passos:

1.  O autor do conteúdo cria um documento e utiliza a aplicação activada pelo RMS para especificar utilizadores e aplicar direitos e condições ao conteúdo.
2.  A aplicação activada pelo RMS gera uma chave de conteúdo simétrica e envia um pedido de licença de publicação ao servidor de certificados ou de licenciamento. O pedido inclui a chave de conteúdo e as definições de utilização.
3.  O servidor de licenciamento gera a licença de publicação, encripta a chave de conteúdo com a chave pública de servidor e, em seguida, devolve a licença de publicação à aplicação activada pelo RMS.
4.  A aplicação encripta o ficheiro com a chave de conteúdo e associa a licença de publicação ao ficheiro.
5.  A aplicação activada pelo RMS do computador do consumidor do conteúdo envia ao servidor do RMS (que emitiu a licença de publicação) um pedido que inclui o certificado de conta de direitos do consumidor, visando pedir uma licença de utilização para o documento.
6.  O servidor do RMS valida as credenciais do utilizador. Se o utilizador for validado com êxito, é gerada e devolvida uma licença de utilização à aplicação activada pelo RMS existente no computador do consumidor do conteúdo.
7.  A aplicação activada pelo RMS abre o documento e concede direitos ao utilizador consoante os parâmetros definidos na licença de utilização.
