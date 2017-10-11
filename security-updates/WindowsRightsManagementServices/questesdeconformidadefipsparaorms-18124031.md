---
TOCTitle: Questões de Conformidade FIPS para o RMS
Title: Questões de Conformidade FIPS para o RMS
ms:assetid: '720bdace-dcd8-431e-b0fa-01193782fe0b'
ms:contentKeyID: 18124031
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747551(v=WS.10)'
---

Questões de Conformidade FIPS para o RMS
========================================

Os Serviços de Gestão de Direitos (RMS) versão 1.0 Service Pack 1 (SP1) foram concebidos para funcionarem eficazmente em organizações que utilizam funcionalidade criptográfica com avaliação FIPS.

A Federal Information Processing Standard 140-1 (FIPS 140-1) e a sua sucessora FIPS 140-2 são normas do Governo dos Estados Unidos que fornecem uma referência para a implementação de software criptográfico. Especificam os procedimentos recomendados para a implementação de algoritmos criptográficos, processamento de material de chaves e memórias intermédias de dados, e utilização do sistema operativo.

O RMS pode ser implementado como parte de um sistema compatível com FIPS para fornecer um meio de protecção dos dados confidenciais.

-   Os fornecedores de serviços criptográficos com avaliação FIPS restringem a funcionalidade a: **TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA**. Esta restrição força o fornecedor do canal de segurança a negociar apenas o protocolo Transport Layer Security (TLS) 1.0 mais seguro. Pode ser necessário configurar o Internet Explorer para suportar o TLS. No entanto, um grande número de servidores Web de terceiros não suporta TLS. Para mais informações sobre estas questões, consulte o artigo 811834 da Base de Dados de Conhecimento no [Web site da Microsoft](http://go.microsoft.com/fwlink/?linkid=43614).

Proteja a chave privada do RMS com um dos dois fornecedores de serviços criptográficos (CSPs) predefinidos da Microsoft, se pretender utilizar protecção de chave privada baseada em software. Estes CSPs concluíram o processo de avaliação FIPS 140-1 ou FIPS 140-2 (conforme adequado) do Governo dos Estados Unidos. Embora tal não seja necessário, recomenda-se que os clientes críticos de segurança utilizem módulos de segurança por hardware (como os da nCipher ou da IBM) para protegerem chaves privadas de nível elevado do servidor do RMS. Se forem utilizados HSMs, o CSP adequado deve ser seleccionado para utilizar o HSM. Isto pode requerer o reinício do sistema. Para mais informações sobre estas questões, consulte o artigo 830690 da Base de Dados de Conhecimento no [Web site da Microsoft](http://go.microsoft.com/fwlink/?linkid=44138).

Quando implementar o sistema do RMS, deve efectuar as seguintes selecções:

-   Siga as directrizes NSA para a criptografia compatível com FIPS no Windows.
-   Active a Política de Segurança Local para a criptografia compatível com FIPS.
-   Implemente os clientes e os servidores do RMS SP1 no ambiente acima.
-   Active o protocolo Transport Layer Security (TLS) nos Serviços de Informação Internet no servidor do RMS.
-   Active o protocolo Transport Layer Security (TLS) no Internet Explorer para os clientes.
-   Active o protocolo Tabular Data Stream (TDS) do SQL utilizado com o Fornecedor de Segurança TLS/SSL do Windows entre os clientes do SQL e o SQL Server do servidor de bases de dados.
-   Configurar o SQL para Requerer TSL/SSL
