---
TOCTitle: Aplicações Activadas pelo RMS
Title: Aplicações Activadas pelo RMS
ms:assetid: '30bb5565-81d3-43d9-a64d-cf0c5b990712'
ms:contentKeyID: 18123928
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720231(v=WS.10)'
---

Aplicações Activadas pelo RMS
=============================

Para criarem ou consumirem conteúdo protegido pelo RMS, os utilizadores têm de ter uma aplicação activada pelo RMS instalada, como descrito neste tópico. O cliente do RMS tem também de estar instalado e os computadores utilizados têm de estar activados. Para mais informações, consulte "[Cliente de RMS](https://technet.microsoft.com/03294fa2-8350-430d-b4b0-03d5169937c2)" e "[Activação de Computador do RMS](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)" posteriormente nesta secção.

As aplicações activadas pelo RMS permitem aos autores de conteúdo anexarem direitos de utilização na forma de licenças de publicação aos ficheiros que criam para controlarem o modo como o conteúdo é consumido. As aplicações activadas pelo RMS processam também as informações dos ficheiros encriptados, permitindo aos utilizadores consumirem o conteúdo de acordo com as permissões definidas na licença de publicação.

A utilização do RMS SDK permite aos programadores criarem aplicações activadas pelo RMS que licenciam, publicam e consomem conteúdo protegido pelo RMS. As aplicações activadas pelo RMS podem ser programadas para computadores com o Microsoft® Windows® 98 Second Edition ou posterior.

Os programadores podem também criar aplicações de servidor activadas pelo RMS utilizando o Rights Management Services Client SDK. Essas aplicações podem publicar conteúdo, mas não consumi-lo.

Os utilizadores, que não têm outra aplicação activada pelo RMS para consumirem conteúdo protegido pelo RMS em mensagens de correio electrónico e páginas Web, podem obter e utilizar o Suplemento de Gestão de Direitos para o Microsoft® Internet Explorer. Por exemplo, os clientes do Outlook Web Access (OWA) podem utilizar o Suplemento de Gestão de Direitos para consumirem mensagens de correio electrónico protegidas pelo RMS.

Pode transferir o Suplemento de Gestão de Direitos para o Internet Explorer a partir do [Web site da Microsoft](http://go.microsoft.com/fwlink/?linkid=14450) (http://go.microsoft.com/fwlink/?LinkId=14450).

| ![](images/Cc720231.note(WS.10).gif)Nota                                                                                                                                                    |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se estiver a utilizar o Suplemento de Gestão de Direitos para o Internet Explorer com o Windows XP Service Pack 2, a configuração de segurança avançada pode criar alguns problemas de compatibilidade entre aplicações. |

Se o URL de ligação da extranet para cada domínio da organização não for adicionado aos sites de Intranet Local no Internet Explorer, os utilizadores com o Suplemento de Gestão de Direitos para o Internet Explorer receberão repetidamente mensagens que solicitam confirmação para a ligação aos sites. Uma resposta incorrecta a estas mensagens pode fazer com que o cliente do RMS obtenha um novo certificado de conta de direitos para a conta de utilizador.

Para definir estes sites correctamente em toda a organização, utilize um script para escrever os URL necessários no registo como parte da zona da Intranet Local. A zona da Intranet Local fornece um nível de segurança predefinido suficientemente alto para eliminar as mensagens.
