---
TOCTitle: Adicionar e Remover Domínios de Publicação Fidedignos
Title: Adicionar e Remover Domínios de Publicação Fidedignos
ms:assetid: 'd87b502d-5497-4ccd-badf-f6807d587cee'
ms:contentKeyID: 18124216
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747687(v=WS.10)'
---

Adicionar e Remover Domínios de Publicação Fidedignos
=====================================================

Por predefinição, um servidor do RMS só poderá emitir licenças de utilização referentes às licenças de publicação emitidas por ele ou por outro servidor do seu cluster. Se tiver conteúdo publicado com outro servidor de certificações de raiz dentro da sua organização, por exemplo, uma subsidiária noutra floresta, ou noutra organização separada, o servidor do RMS poderá conceder licenças de utilização a utilizadores para este conteúdo se configurar um domínio de publicação fidedigno no servidor do RMS. Quando adicionar um domínio de publicação fidedigno, é necessário configurar uma relação de fidedignidade entre o servidor do RMS e o outro servidor de certificações de raiz, importando o certificado de licenciador de servidores do outro servidor. Não há limite para o número de domínios de publicação fidedignos que pode configurar para o servidor do RMS.

Pode remover, em qualquer altura, um domínio de publicação fidedigno que tenha sido adicionado, bastando para tal remover o respectivo certificado da lista de certificados de domínios de publicação fidedignos.

Para adicionar um domínio de publicação fidedigno, é necessário importar o certificado de licenciador de servidores , a chave privada (se a chave privada estiver guardada no software e não num módulo de segurança por hardware) e todos os modelos de política de direitos do servidor ou do cluster do RMS que pretende adicionar. O administrador tem primeiro de exportar esses itens do servidor ou do cluster fidedigno para um ficheiro protegido por palavra-passe, tendo depois de especificar a palavra-passe necessária para o desencriptar. O administrador deverá colocar esse ficheiro numa pasta partilhada e comunicar-lhe a palavra-passe. Depois, pode importar o ficheiro, especificando a respectiva localização e palavra-passe. Para guardar o ficheiro, a conta que está a executar o grupo de aplicações **Admin** deverá dispor de permissões para a pasta partilhada.

Para ver instruções detalhadas para estabelecer um domínio de publicação fidedigno, consulte "[Para Adicionar um Domínio de Publicação Fidedigno](https://technet.microsoft.com/731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c)" posteriormente nesta secção.

Se a chave privada estiver guardada num módulo de segurança por hardware, é necessário transferir a chave privada para o módulo de segurança por hardware que se encontra no servidor fidedigno seguindo as instruções existentes na documentação do módulo de segurança por hardware. Dependendo do módulo de segurança por hardware que se encontra em cada servidor e da configuração dos dispositivos do módulo de segurança por hardware, poderá não ser possível transferir a chave privada de um módulo de segurança por hardware para outro. Consulte a documentação do módulo de segurança por hardware para determinar se pode transferir a chave privada sem perder dados que se encontram no módulo de segurança por hardware de destino. Se não for possível transferir com segurança a chave privada, não é possível estabelecer um domínio de publicação fidedigno entre os dois servidores.

| ![](images/Cc747687.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                           |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se estiver a utilizar um módulo de segurança por hardware para proteger a chave privada do RMS e importar um certificado de licenciador de servidores de uma instalação do RMS que utilize protecção de chave privada por meio de software, é necessário especificar uma palavra-passe da chave privada na página de Definições de segurança do servidor RMS no cluster antes de tentar importar o certificado. |
