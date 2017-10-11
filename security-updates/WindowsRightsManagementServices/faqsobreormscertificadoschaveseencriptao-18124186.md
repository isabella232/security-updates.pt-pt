---
TOCTitle: 'FAQ sobre o RMS: Certificados, Chaves e Encriptação'
Title: 'FAQ sobre o RMS: Certificados, Chaves e Encriptação'
ms:assetid: 'ad8cc088-1dea-44c2-be68-9091129f0f12'
ms:contentKeyID: 18124186
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747725(v=WS.10)'
---

FAQ sobre o RMS: Certificados, Chaves e Encriptação
===================================================

Perguntas Mais Frequentes Sobre a Certificados, Chaves e Encriptação
--------------------------------------------------------------------

-   [Quais são os algoritmos de encriptação utilizados no RMS?](#bkmk_10)
-   [O RMS utiliza encriptação certificada pela FIPS?](#bkmk_11)
-   [Para modelos ou licenças de publicação que concedam permissões a uma lista de distribuição em vez de utilizadores individuais, as licenças de utilização são processadas de forma diferente para avaliar os membros dinamicamente?](#bkmk_12)
-   [Quando o RMS for utilizado a partir de um quiosque, é emitido um certificado de conta de direitos (RAC) temporário. Qual é a diferença entre um RAC temporário e um RAC padrão? Como é que o RMS detecta que está ser utilizado num quiosque?](#bkmk_13)
-   [Quando é utilizado um RAC temporário?](#bkmk_14)
-   [O RMS emite certificados X.509v3?](#bkmk_15)
-   [Em que local são guardados os certificados XrML?](#bkmk_16)
-   [Em que local é guardado o par da chave pública/privada da máquina?](#bkmk_17)
-   [Em que local é guardado o par da chave pública/privada do cliente?](#bkmk_18)
-   [O AES é um algoritmo simétrico. Como são transmitidas as chaves em segurança entre o servidor e o utilizador?](#bkmk_19)

<span id="BKMK_10"></span>
#### Quais são os algoritmos de encriptação utilizados no RMS?

O RMS utiliza chaves RSA de 2048 bits para o servidor do RMS e chaves RSA de 1024 bits para o par da chave da máquina e do utilizador.

<span id="BKMK_11"></span>
#### O RMS utiliza encriptação certificada pela FIPS?

No RMS com Service Pack 1 e posteriores, os cofres gerados pela aplicação do cliente do RMS utiliza a encriptação AES certificada pela FIPS quando o cliente estiver instalado num computador com o Windows XP ou o Windows Server 2003. No entanto, se o cliente do RMS estiver instalado em computadores com o Windows 2000, não é instalada a biblioteca AES certificada pela FIPS e os cofres não são compatíveis com FIPS.

<span id="BKMK_12"></span>
#### Para modelos ou licenças de publicação que concedam permissões a uma lista de distribuição em vez de utilizadores individuais, as licenças de utilização são processadas de forma diferente para avaliar os membros dinamicamente?

As licenças de utilização são sempre emitidas para utilizadores individuais. Se um modelo ou uma licença de publicação nomear um grupo, o RMS avalia os membros do grupo no momento da emissão da licença de utilização. Se o utilizador que requer a licença for um membro do grupo nomeado, a licença de utilização é emitida para a identidade do utilizador.

<span id="BKMK_13"></span>
#### Quando o RMS for utilizado a partir de um quiosque, é emitido um certificado de conta de direitos (RAC) temporário. Qual é a diferença entre um RAC temporário e um RAC padrão? Como é que o RMS detecta que está ser utilizado num quiosque?

A aplicação activada pelo RMS deverá determinar se o cliente do RMS deve requerer um RAC temporário ou RAC padrão para o utilizador. Não existe qualquer método de detecção para esta situação. O Microsoft Office 2003 é um exemplo de uma aplicação activada pelo RMS que permite ao utilizador seleccionar o RAC adequado.

A diferença principal entre um RAC temporário e um RAC padrão é a presença do identificador de segurança do utilizador e a especificação do prazo de validade. Os RACs temporários não incluem a SID do utilizador e têm um prazo de validade especificado em número de minutos. O prazo de validade predefinido para um RAC temporário é de 15 minutos. No entanto, os RACs padrão não incluir a SID do utilizador e têm um prazo de validade especificado em número de dias. O prazo de validade predefinido para um RAC padrão é de 365 dias.

<span id="BKMK_14"></span>
#### Quando é utilizado um RAC temporário?

Um RAC temporário é concebido para permitir que um utilizador consuma conteúdo protegido pelo RMS em computadores que satisfaçam qualquer um dos seguintes critérios:

-   Um computador que não seja membro da mesma floresta da instalação do RMS em que o RAC foi obtido.
-   Um computador que não seja membro da mesma floresta em que a conta do utilizador está localizada.
-   O utilizador não tem a certeza de que vai utilizar o mesmo computador posteriormente.

Os exemplos de computadores que se encaixam nestes critérios podem ser encontrados em terminais de aeroportos, bibliotecas públicas e cibercafés.

<span id="BKMK_15"></span>
#### O RMS emite certificados X.509v3?

Não. O RMS emite certificados XrML destinados a representar utilizadores e uma expressão política que está para além do âmbito dos certificados X.509v3.

<span id="BKMK_16"></span>
#### Em que local são guardados os certificados XrML?

Um sistema RMS utiliza os certificados e as licenças seguintes guardados em XrML no computador cliente.

-   Certificado do computador
    Nome do ficheiro: Ficheiro CERT-Machine.drm
    Localização: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM\\
-   Certificado de conta de direitos
    Prefixo do nome do ficheiro: GIC
    Localização: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM
-   Certificado de cliente licenciador
    Prefixo do nome do ficheiro: CLC
    Localização: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM
-   Licença de utilização
    Prefixo do nome do ficheiro: EUL
    Localização: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM

| ![](images/Cc747725.note(WS.10).gif)Nota                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Uma conta de utilizador tem um certificado de computador, um ficheiro GIC e um ficheiro CLC, mas vários ficheiros EUL para cada parte de conteúdo a que se acede. |

| ![](images/Cc747725.note(WS.10).gif)Nota                                                |
|----------------------------------------------------------------------------------------------------------------------|
| Para o cliente do RMS integrado com o Windows Vista®, a localização é %USERPROFILE%\\AppData\\Local\\Microsoft\\DRM. |

<span id="BKMK_17"></span>
#### Em que local é guardado o par da chave pública/privada da máquina?

A chave privada do computador é guardada em segurança, protegida pelas chaves criptográficas relacionadas com as credenciais de início de sessão do utilizador e a configuração do computador.

<span id="BKMK_18"></span>
#### Em que local é guardado o par da chave pública/privada do cliente?

O par de chaves para uma conta de utilizador é guardada no certificado de conta de direitos.

<span id="BKMK_19"></span>
#### O AES é um algoritmo simétrico. Como são transmitidas as chaves em segurança entre o servidor e o utilizador?

As chaves privadas/públicas e simétricas são utilizadas no sistema. O conteúdo é encriptado com uma chave simétrica, mas as outras chaves do sistema (utilizador, computador e servidor) são chaves privadas/públicas RSA. A chave de conteúdo simétrica está sempre encriptada nas várias licenças — quer seja a chave pública RSA do servidor do RMS ou a chave pública RSA do utilizador na licença de utilização.
