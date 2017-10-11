---
TOCTitle: 'FAQ sobre o RMS: Acesso Interno e Externo'
Title: 'FAQ sobre o RMS: Acesso Interno e Externo'
ms:assetid: '59c2c51f-6c20-450c-a334-0e1486292074'
ms:contentKeyID: 18124023
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747577(v=WS.10)'
---

FAQ sobre o RMS: Acesso Interno e Externo
=========================================

Perguntas Mais Frequentes Sobre o Acesso Interno e Externo do RMS
-----------------------------------------------------------------

-   [Que alterações tenho de fazer para a minha firewall permitir o acesso de clientes RMS exteriores à firewall aos servidores do RMS?](#bkmk_37)
-   [Como é que funciona o cenário da extranet?](#bkmk_38)
-   [Se um utilizador criar o conteúdo protegido por direitos e o fornecer a alguém que não tenha acesso à instalação do RMS, o destinatário pode utilizar o conteúdo?](#bkmk_39)
-   [Se utilizar o Outlook 2003 ou Outlook 2007 para enviar uma mensagem de correio electrónico protegida por direitos para um dos meus clientes, o que é necessário para ler o correio?](#bkmk_40)
-   [Se as organizações tiverem servidores do RMS próprios, como é que podem trocar conteúdo protegido por direitos?](#bkmk_41)
-   [Quando enviar uma mensagem de correio electrónico que tenha sido protegida com o RMS para uma organização exterior que não suporte o Outlook, o destinatário pode responder a uma mensagem de correio que tenha sido lida utilizando o Suplemento de Gestão de Direitos com o Internet Explorer?](#bkmk_42)

<span id="BKMK_37"></span>
#### Que alterações tenho de fazer para a minha firewall permitir o acesso de clientes RMS exteriores à firewall aos servidores do RMS?

A firewall deverá permitir aos computadores exteriores fazerem pedidos de protocolo SOAP (Simple Object Access Protocol) ao servidor do RMS sobre HTTP (TCP porta 80) ou HTTPS (TCP porta 443).

<span id="BKMK_38"></span>
#### Como é que funciona o cenário da extranet?

Estão contidos dois URLs na licença de publicação associada ao conteúdo. Um é o URL da intranet definido quando o cluster do RMS é aprovisionado. O segundo é o URL de uma extranet que pode ser definido pelo administrador do RMS. Este URL da extranet permite ao cliente obter licenças de utilização fora da firewall. O URL da extranet não pode ser utilizado para criar novo conteúdo protegido por direitos. Nesse caso, é necessária a substituição do registo do cliente do RMS.

<span id="BKMK_39"></span>
#### Se um utilizador criar o conteúdo protegido por direitos e o fornecer a alguém que não tenha acesso à instalação do RMS, o destinatário pode utilizar o conteúdo?

Se o utilizador não tiver uma ligação à instalação do RMS quando o conteúdo protegido for aberto pela primeira vez, o utilizador não pode utilizar o conteúdo.

Não se esqueça de que o Office 2003 e posteriores obtêm automaticamente as licenças de utilização para o correio electrónico protegido por direitos aquando da sincronização, para que o correio electrónico possa ser lido sem uma ligação à rede. No entanto, enquanto o Outlook 2003 e posteriores colocam em cache automaticamente as licenças de utilização para uma mensagem de correio electrónico, qualquer documento Excel 2007, Excel 2003, Word 2007, Word 2003, PowerPoint 2007 e PowerPoint 2003 anexado à mensagem de correio electrónico tem os mesmos direitos atribuídos à mensagem de correio electrónico que o transporta. A sincronização não é efectuada automaticamente quando o correio electrónico é transferido e deve abrir-se individualmente quando o computador é ligado à rede para obter uma licença de utilização.

<span id="BKMK_40"></span>
#### Se utilizar o Outlook 2003 ou Outlook 2007 para enviar uma mensagem de correio electrónico protegida para um dos meus clientes, o que é necessário para ler o correio?

O destinatário necessita de utilizar o Outlook 2003, Outlook 2007 ou o Suplemento de Gestão de Direitos com o Internet Explorer. Se a organização do destinatário estabeleceu uma relação fidedigna entre a sua instalação do RMS e a instalação do RMS do emissor, o destinatário pode ler o correio electrónico sem passos adicionais. A relação de fidedignidade é estabelecida através da troca de certificados de servidor licenciador do RMS, que contêm as respectivas chaves públicas.

Se a organização do destinatário não tiver uma infra-estrutura de RMS ou não houver uma relação de fidedignidade estabelecida, pode pedir ao cliente para criar um Windows Live ID e, em seguida, enviar uma mensagem de correio electrónico ao destinatário especificando os direitos atribuídos às credenciais da conta Windows Live ID do cliente. Esta abordagem utiliza o Serviço IRM da Microsoft disponível na Internet para obter uma licença de utilização. O Serviço IRM é fornecido gratuitamente para permitir que as pessoas utilizem o IRM para efeitos de teste e destina-se apenas ao teste do RMS. Se quiser proteger o conteúdo com este serviço, não se esqueça de que este pode ser descontinuado sem aviso prévio.

<span id="BKMK_41"></span>
#### Se as organizações tiverem servidores do RMS próprios, como é que podem trocar conteúdo protegido por direitos?

O RMS utiliza domínios de utilizadores fidedignos em que os certificados dos utilizadores gerados por uma instalação do RMS são considerados fidedignos por outra.

<span id="BKMK_42"></span>
#### Quando enviar uma mensagem de correio electrónico que tenha sido protegida com o RMS para uma organização exterior que não suporte o Outlook, o destinatário pode responder a uma mensagem de correio que tenha sido lida utilizando o Suplemento de Gestão de Direitos com o Internet Explorer?

O destinatário do correio electrónico pode responder a uma mensagem de correio electrónico protegida por direitos de uma forma normal, mas o corpo original da mensagem de correio electrónico recebida permanecerá protegido por direitos para os destinatários originais. A forma como a mensagem de correio electrónico é compactada depende da aplicação do cliente. A mensagem de correio electrónico original pode ser anexada à resposta como um anexo encriptado ou poderá ser removida, como acontece, por exemplo, no Outlook 2003 ou Outlook 2007.
