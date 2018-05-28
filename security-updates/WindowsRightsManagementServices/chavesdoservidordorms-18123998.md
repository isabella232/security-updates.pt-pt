---
TOCTitle: Chaves do Servidor do RMS
Title: Chaves do Servidor do RMS
ms:assetid: '5f4100a1-9aa5-42af-85c8-4bc691022f06'
ms:contentKeyID: 18123998
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720280(v=WS.10)'
---

Chaves do Servidor do RMS
=========================

Um servidor do RMS tem um par de chaves das chaves RSA de 1024 bits.

A chave pública do servidor é utilizada na encriptação da chave de conteúdo existente na licença de publicação para que apenas o servidor do RMS possa obter a chave do conteúdo e emitir licenças de utilização associadas à licença de publicação. O certificado de licenciador de servidores contém a chave pública do servidor.

A chave privada do servidor é utilizada para assinar todos os certificados e licenças emitidos pelo servidor.

Protecção da chave privada do servidor
--------------------------------------

Por predefinição, durante o aprovisionamento, a chave privada do servidor é criada e armazenada na base de dados do RMS em forma encriptada. Em alternativa, durante o aprovisionamento, pode especificar um fornecedor de serviços criptográficos (CSP) que já esteja instalado no servidor.

Pode utilizar um CSP de duas formas diferentes:

-   Escolher entre implementações de CSP por software que são instaladas, por predefinição, com o servidor.
    - ou -
-   Utilize um CSP de software não-Microsoft instalado no servidor.

| ![](/security-updates/images/Cc720280.note(WS.10).gif)Nota                                                                       |
|---------------------------------------------------------------------------------------------------------------------------------------------|
| Se desejar utilizar um módulo de segurança por hardware, certifique-se de que escolhe um CSP que suporte módulos de segurança por hardware. |

Se optar por proteger a chave privada do servidor através de um CSP, o RMS armazena o nome do fornecedor e o nome do contentor de chaves da base de dados de configuração.
