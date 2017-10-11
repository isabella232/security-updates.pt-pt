---
TOCTitle: Excluir Aplicações
Title: Excluir Aplicações
ms:assetid: 'b68ae4b2-b9ba-44ae-90cb-c88df600ec86'
ms:contentKeyID: 18124151
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747644(v=WS.10)'
---

Excluir Aplicações
==================

Pode especificar a versão de uma aplicação activada pelo RMS, contra a qual todos os pedidos de licenciamento tenham de ser confrontados. A exclusão de aplicações marca cada licença de utilização com uma condição, que especifica que a licença só pode ser associada ao conteúdo protegido pelo RMS para o qual foi emitida se a aplicação que está a solicitar a licença não se encontrar na lista de exclusões.

Isto pode ser útil, por exemplo, quando uma empresa implementa uma actualização de segurança para uma aplicação. Os administradores de sistema podem utilizar o seu mecanismo habitual para fazer com que os computadores cliente instalem a actualização de segurança. Poderão então definir as políticas de exclusão de aplicações definidas utilizando as informações de versão da aplicação que está a utilizar o Web site de administração. Esta política de exclusão restringe a emissão de licenças pelo RMS para clientes que estejam a utilizar versões anteriores do software.

As aplicações activadas pelo RMS são excluídas através do respectivo nome de ficheiro e número de versão. Pode ser útil fazer isto para ter a certeza de que os utilizadores instalam uma versão mais recente e mais segura de uma aplicação assim que ela fica disponível. Por exemplo, poderá ter a versão 1.0.4.2315 de uma aplicação activada pelo RMS implementada na sua organização. Depois, o programador de aplicações descobre um problema de segurança e emite a versão 1.0.4.4200, que elimina o problema. Além de implementar a nova versão da aplicação, poderá estabelecer uma política de exclusão que impeça os utilizadores de consumirem conteúdos protegidos utilizando a versão anterior da aplicação.

À semelhança do que acontece com outros tipos de exclusão, é necessário configurar a exclusão da aplicação em cada cluster onde se pretenda que ela entre em vigor.

Quando aplicar esta política de exclusão no servidor, os clientes não poderão utilizar a aplicação excluída para solicitar e associar novas licenças de utilização a conteúdo protegido pelo RMS. No entanto, os clientes podem continuar a utilizar a aplicação excluída para consumir ficheiros licenciados anteriormente.

| ![](images/Cc747644.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                    |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| O RMS requer que especifique a versão da aplicação num formato de 4 dígitos delimitados por pontos (\#.\#.\#.\# ). No entanto, algumas aplicações especificam a respectiva versão através de um número de 2 ou 3 dígitos delimitado por pontos. Neste caso, deverá adicionar um .0 conforme adequado para corresponder o número da versão ao formato requerido pelo RMS. |
