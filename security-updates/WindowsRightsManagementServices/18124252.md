---
TOCTitle: Publicação Offline
Title: Publicação Offline
ms:assetid: 'f6384ed2-f917-442e-aa63-c1394a1c4d06'
ms:contentKeyID: 18124252
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747741(v=WS.10)'
---

Publicação Offline
==================

A publicação offline é diferente da publicação online devido à forma como a aplicação activada pelo RMS adquire a licença de publicação.

Antes de um autor publicar conteúdo offline, necessita de adquirir um certificado de licenciador de clientes enquanto tem acesso ao servidor de certificações de raiz através da rede.

O processo de publicação offline envolve os seguintes passos:

1.  O autor cria o documento utilizando uma aplicação activada pelo RMS e, em seguida, especifica os direitos e as condições do conteúdo.
2.  Quando o autor guarda o ficheiro, o certificado de licenciador de clientes permite ao computador ou ao dispositivo local emitir e assinar uma licença de publicação para o ficheiro.
    A licença de publicação contém duas cópias da chave de conteúdo: uma que está encriptada com a chave pública do certificado de licenciador de clientes, e outra que está encriptada com a chave pública do servidor que emitiu o certificado de licenciador de clientes. Também contém o URL do servidor. As duas chaves públicas e o URL provêm do certificado de licenciador de clientes.
3.  O computador utiliza o certificado de licenciador de clientes para criar uma licença de proprietário. Esta é uma licença de utilização especial que concede ao autor o direito de consumir conteúdo protegido pelo RMS quando está offline. O certificado de licenciador de clientes utiliza a respectiva chave privada para desencriptar a chave de conteúdo simétrica da licença de publicação e, em seguida, volta a encriptá-la para a licença de proprietário.
4.  A aplicação encripta o ficheiro com a chave de conteúdo e associa a licença de publicação ao ficheiro. Apenas o servidor do RMS que emitiu a licença de publicação ou um servidor que é um membro de um domínio de publicação fidedigno pode emitir licenças que desencriptem o ficheiro.
