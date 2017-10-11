---
TOCTitle: Planear os Utilizadores Externos do RMS
Title: Planear os Utilizadores Externos do RMS
ms:assetid: '107e1338-4dcf-4ed5-a49d-e875cc883db1'
ms:contentKeyID: 18123901
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720190(v=WS.10)'
---

Planear os Utilizadores Externos do RMS
=======================================

Esta secção descreve as topologias que pode implementar para que a organização e os utilizadores externos partilhem conteúdo protegido pelo RMS na Internet.

Pode implementar clusters do RMS para utilização interna e externa utilizando uma das seguintes opções:

-   Defina o URL do cluster de certificações de raiz para um URL que possa ser acedido na Internet. Certifique-se de que este URL é resolvido na intranet para os servidores do RMS pertencentes ao mesmo cluster. Quando utiliza esta opção, o URL da licença de publicação utilizado por computadores de utilizador final para a aquisição da licença funciona na intranet e na Internet.
-   Configure um cluster separado do RMS dedicado à publicação na Internet. Qualquer conteúdo que tenha de ser licenciado a partir da Internet deve ser publicado neste cluster. Se o conteúdo tiver de ficar disponível tanto interna como externamente, deve ser publicado em ambos os locais. Como alternativa, os utilizadores têm de conseguir contactar o servidor de Internet.

Permitir Utilizadores Externos
------------------------------

Pode incluir utilizadores externos na instalação do RMS se criar contas internas para esses utilizadores e permitir que estes obtenham acesso à rede da empresa através de uma rede privada virtual (VPN). A conta pode ter uma caixa de correio interna ou um endereço de correio electrónico direccionado para uma caixa de correio externa.

Se utilizar uma caixa de correio interna, os autores internos têm de especificar um endereço de correio electrónico associado a essa caixa de correio interna (e não qualquer endereço de correio electrónico associado ao utilizador externo fora da organização) quando publicam conteúdo protegido pelo RMS. Se utilizar uma caixa de correio externa, os autores internos têm de especificar o endereço de correio electrónico externo da conta quando publicam conteúdo protegido pelo RMS.

Para fornecer segurança de rede e fornecer suporte de acesso de rede a utilizadores externos, pode criar uma floresta separada do Active Directory para contas de parceiro. Esta topologia permite a criação de um cluster de certificações de raiz separado para o lado de Internet do sistema do RMS. Isto permite aos utilizadores externos receberem os respectivos certificados de computador e de contas de direitos do RMS a partir do cluster de certificações de raiz do lado da Internet quando obtêm acesso pela primeira vez a conteúdo protegido pelo RMS.

Se optar por implementar uma floresta separada para parceiros externos que irá conter as contas de parceiros, tem de instalar o RMS nessa floresta. Em seguida, utilize a funcionalidade de domínio de publicação fidedigno para estabelecer uma relação de fidedignidade entre os dois servidores do RMS. Necessita também que os registos de DNS externos identifiquem o URL do cluster externo da instalação do RMS na floresta criada para os parceiros externos. A criação desta relação de fidedignidade permite ao servidor externo do RMS emitir licenças de utilização para todo o conteúdo emitido pelo sistema interno do RMS e vice-versa.

Como alternativa à configuração de um servidor do RMS na floresta externa, pode utilizar um servidor como o servidor ISA para filtrar o tráfego recebido e inverter os pedidos de licença no proxy do RMS para o servidor interno do RMS.

Utilizar Certificados Externos
------------------------------

Pode permitir aos utilizadores externos obterem acesso a conteúdo protegido pelo RMS se configurar um servidor separado do RMS como um servidor de licenciamento do lado da Internet, publicar o conteúdo a partir desse servidor de licenciamento e, em seguida, especificar relações de fidedignidade para esse servidor.

O lado da Internet da implementação do RMS é um servidor de licenciamento separado dedicado à utilização na Internet. Faz parte do mesmo cluster que a instalação de licenciamento interna, e utiliza a mesma base de dados e o mesmo URL que a instalação de licenciamento interna; é o único servidor que pode aceitar tráfego proveniente da Internet.

Quando os utilizadores externos pedem uma licença de utilização a partir deste servidor de licenciamento do RMS, utilizam um Certificado de Conta de Direitos de outro serviço de certificação do RMS considerado como fidedigno pelo serviço de certificação do RMS.

#### Considerar Fidedignos os Certificados de Contas de Direitos Baseados no Passport

A organização pode optar por considerar fidedignos os certificados de contas de direitos baseados em credenciais do Microsoft .NET Passport. Estes certificados de contas requerem que os utilizadores obtenham certificados de contas de direitos directamente no Serviço de Certificação da Microsoft alojado na Internet.

Neste modelo, os utilizadores externos recebem certificados de computador do RMS e certificados de contas de direitos a partir da Microsoft. Quando o conteúdo é publicado, o utilizador externo da conta do Microsoft .NET Passport tem de ser designado como um destinatário da licença de publicação.

A conta do Microsoft® .NET Passport tem de corresponder à conta do .NET Passport utilizada quando o utilizador transferiu o certificado de conta de direitos da Microsoft. O autor tem de especificar esta conta quando adiciona os destinatários na aplicação activada pelo RMS. Se as contas não coincidirem, o conteúdo não pode ser consumido.

#### Considerar Fidedignos Outros Certificados Externos

Se a empresa do utilizador externo também tem uma implementação do RMS, pode optar por configurar uma relação de fidedignidade com essa empresa. Para tal, peça à empresa para exportar o respectivo certificado de licenciador de servidores do RMS e lho enviar. Em seguida, pode importar o certificado utilizando a consola de administração do RMS para o servidor de licenciamento do lado da Internet.
