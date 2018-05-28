---
TOCTitle: Retirar Modelos de Política de Direitos
Title: Retirar Modelos de Política de Direitos
ms:assetid: '32bf98c7-edda-4507-a4b8-4c11bddd6e60'
ms:contentKeyID: 18123932
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720239(v=WS.10)'
---

Retirar Modelos de Política de Direitos
=======================================

Para retirar um modelo de política de direitos tem de o eliminar. Este procedimento é descrito em “[Para Eliminar um Modelo de Política de Direitos](https://technet.microsoft.com/9c9a1496-cf55-4c65-a4c6-9fe245edce00)” posteriormente nesta secção. No entanto, normalmente os modelos de política de direitos não devem ser eliminados. Se pretender mesmo retirar um modelo de política de direitos, tem de ter o cuidado de não se esquecer de remover as cópias desse modelo que existem nos computadores dos utilizadores. Deve fazê-lo porque é enviado para o servidor do RMS um pedido quando um autor utiliza um modelo de política de direitos para publicar conteúdos. O RMS utiliza uma cópia do modelo de política de direitos que está guardado na base de dados para responder ao pedido. Se o modelo de política de direitos não existir na base de dados, o pedido falha.

| ![](/security-updates/images/Cc720239.note(WS.10).gif)Nota                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Uma das formas de gerir o modo como se retira um modelo de política de direitos consiste em criar um script que remova esse modelo de todos os computadores dos utilizadores. |
