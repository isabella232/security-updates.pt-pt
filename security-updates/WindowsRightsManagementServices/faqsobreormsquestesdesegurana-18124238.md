---
TOCTitle: 'FAQ sobre o RMS: Questões de Segurança'
Title: 'FAQ sobre o RMS: Questões de Segurança'
ms:assetid: 'ff433834-79aa-481f-bd39-3393be12a26f'
ms:contentKeyID: 18124238
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747757(v=WS.10)'
---

FAQ sobre o RMS: Questões de Segurança
======================================

Perguntas Mais Frequentes Sobre Questões de Segurança no RMS
------------------------------------------------------------

-   [O que é uma conta de super utilizador?](#bkmk_43)
-   [O RMS é uma solução de segurança?](#bkmk_44)
-   [Que mecanismos existem para impedir os destinatários de reverterem o relógio do respectivo computador cliente para ampliar o acesso a um documento protegido por direitos depois de a licença de utilização ter expirado?](#bkmk_45)
-   [É possível aos membros do grupo de Admins do Domínio lerem documentos destinados a alguém no seu domínio?](#bkmk_46)
-   [Compreendo que todos os cofres podem autenticar todos os certificados ou licenças gerados pelo sistema, como se se tratasse de um serviço registado na Microsoft. Esta protecção é contra que as ameaças?](#bkmk_47)
-   [Se alguém conseguir abrir um documento com um ataque de força bruta, esse ataque permitirá abrir outros documentos com essa chave?](#bkmk_48)
-   [Devido às restrições de exportação sobre tecnologias de encriptação, existe alguma parte das chaves exposta ao exterior da empresa que a implementou?](#bkmk_49)
-   [Como impedir os intrusos maliciosos de ligarem a função de desactivação remotamente?](#bkmk_50)
-   [Um utilizador pode efectuar capturas de ecrãs de conteúdo protegido por direitos?](#bkmk_51)
-   [Os administradores que fazem cópias de segurança dos ficheiros relacionados com o RMS podem aceder ao conteúdo protegido por direitos?](#bkmk_52)
-   [O ficheiro de troca utilizado pelo Windows contém o conteúdo não encriptado em algum ponto, deixando potencialmente conteúdo “aberto”?](#bkmk_53)
-   [É possível limitar os administradores que podem aceder às diferentes funcionalidades administrativas do RMS?](#bkmk_54)
-   [O RMS pode proteger documentos individuais assim que forem criados, no disco rígido do utilizador ou numa pasta partilhada?](#bkmk_55)
-   [Quando abrir um ficheiro, o ficheiro de gravação automática e os ficheiros temporários estão encriptados?](#bkmk_56)
-   [Quando recebo uma mensagem de correio electrónico protegida por direitos, parece que existe um anexo incluído na mensagem de correio electrónico. Posso guardar esse anexo mesmo quando não seja supostamente possível guardar o correio - o RMS é quebrado?](#bkmk_562)

<span id="BKMK_43"></span>
#### O que é uma conta de super utilizador?

O RMS suporta um grupo especial de super utilizadores que detém o controlo total sobre todos os conteúdos protegidos por direitos. São concedidos aos membros do grupo de super utilizadores todos os direitos de proprietário para todas as licenças de utilização emitidas pelo cluster do RMS em que o grupo de super utilizadores está configurado. Isto significa que os membros deste grupo podem desencriptar todo e qualquer ficheiro protegido, bem como remover a protecção desses ficheiros. Um membro deste grupo pode, por exemplo, remover a protecção de ficheiros que foram publicados por um determinado funcionário de forma a que um novo proprietário possa publicar e gerir os ficheiros.

<span id="BKMK_44"></span>
#### O RMS é uma solução de segurança?

Não, o RMS não é uma solução de segurança. Quando utilizado com uma aplicação activada pelo RMS, como o Office 2007, pode ser considerada como uma “solução de aplicação de políticas.” Se o utilizador não estiver autorizado a ver os dados, o utilizador poderá fazer um ataque de força bruta para tentar quebrar a encriptação. Apesar de a encriptação ser robusta, tal como todos os esquemas de encriptação de software, pode ser quebrada. No entanto, se o utilizador tiver direitos para ver os dados, pode copiá-los ou tirar uma fotografia digital e fornecer as informações a utilizadores não autorizados.

<span id="BKMK_45"></span>
#### Que mecanismos existem para impedir os destinatários de reverterem o relógio do respectivo computador cliente para ampliar o acesso a um documento protegido por direitos depois de a licença de utilização ter expirado?

O RMS detecta se o relógio de um sistema cliente foi atrasado ou adiantado e impede o utilizador de consumir o conteúdo. Além disso, o RMS detecta se existe um diferencial de relógio mensurável entre o cliente e o servidor do RMS.

<span id="BKMK_46"></span>
#### É possível aos membros do grupo de Admins do Domínio lerem documentos destinados a alguém no seu domínio?

Os membros do grupo de Admins do Domínio podem ler conteúdo protegido de uma conta de utilizador se forem membros do grupo de super utilizadores do RMS ou imitarem a conta do utilizador. Como os membros do grupo de Admins do Domínio têm controlo sobre as contas do utilizador no domínio, não existe atenuação para o cenário de um membro desonesto do grupo de Admins do Domínio.

Como procedimento recomendado, adicione os membros do grupo de Admins do Domínio ao grupo de super utilizadores apenas quando necessitarem de aceder ao conteúdo protegido por direitos. Quando é concedida uma licença a um membro do grupo de super utilizadores, é registada uma ID de evento 49 no registo de eventos da Aplicação do servidor do RMS. A ID de evento 49 indica que **“Foi concedida uma licença a um utilizador pertencente ao grupo de super utilizadores. O utilizador tem o endereço de correio electrónico seguinte: &lt;alias do utilizador&gt;”**, em que o **alias do utilizador** é substituído pela conta de correio electrónico do utilizador.

Tal como outros grupos utilizados para limitar o acesso aos recursos, deverá definir alertas e efectuar verificações de segurança para ajudar a impedir alguém de se associar ao grupo de super utilizadores sem autorização.

<span id="BKMK_47"></span>
#### Compreendo que todos os cofres podem autenticar todos os certificados ou licenças gerados pelo sistema, como se se tratasse de um serviço registado na Microsoft. Esta protecção é contra que as ameaças?

Se não for possível verificar a integridade dos certificados, um utilizador pode recorrer ao spoof um certificado de conta de direitos (RAC) emitido para outro utilizador e obter uma licença de utilização do conteúdo, ou criar uma aplicação para remover a protecção de um documento.

<span id="BKMK_48"></span>
#### Se alguém conseguir abrir um documento com um ataque de força bruta, esse ataque permitirá abrir outros documentos com essa chave?

Cada parte do conteúdo protegido por direitos é encriptada com uma chave simétrica diferente e gerada aleatoriamente. Por isso, a chave para cada documento é única e não é útil para desencriptar outros documentos.

<span id="BKMK_49"></span>
#### Devido às restrições de exportação sobre tecnologias de encriptação, existe alguma parte das chaves exposta ao exterior da empresa que a implementou?

As aplicações assinadas na raiz da Microsoft estão sujeitas à raiz de assinatura da chave da Microsoft mas, a partir desse ponto, nenhuma outra chave é apresentada pela Microsoft ou por uma implementação do cliente.

<span id="BKMK_50"></span>
#### Como impedir os intrusos maliciosos de ligarem a função de desactivação remotamente?

O intruso necessitaria das credenciais da conta de um utilizador com direitos administrativos no cluster do RMS. Por predefinição, a interface de administração do RMS só está disponível localmente no servidor do RMS. Desde que este seja o caso, que o protocolo de ambiente de trabalho remoto (RDP) esteja desactivado e que o servidor esteja fisicamente seguro, ajudará a atenuar o risco.

<span id="BKMK_51"></span>
#### Um utilizador pode efectuar capturas de ecrãs de conteúdo protegido por direitos?

Se os direitos do RMS forem definidos para rejeitar a funcionalidade de cópia, o Windows Alt+PrtSc é desactivado pelo RMS. No entanto, num ambiente com computadores de secretária não geridos, um utilizador poderá utilizar produtos não Microsoft para capturar conteúdo.

<span id="BKMK_52"></span>
#### Os administradores que fazem cópias de segurança dos ficheiros relacionados com o RMS podem aceder ao conteúdo protegido por direitos?

Não; podem efectuar as cópias de segurança, mas não têm acesso.

<span id="BKMK_53"></span>
#### O ficheiro de troca utilizado pelo Windows contém o conteúdo não encriptado em algum ponto, deixando potencialmente conteúdo “aberto”?

Assim que o cliente do RMS enviar conteúdo desencriptado para a aplicação, poderá aparecer no ficheiro de troca. Parte das recomendações de desenvolvimento da aplicação RMS no RMS SDK inclui passos para impedir esta ocorrência, mas a execução do procedimento deverá ser efectuada pela aplicação activada pelo RMS.

<span id="BKMK_54"></span>
#### É possível limitar os administradores que podem aceder às diferentes funcionalidades administrativas do RMS?

Sim, pode criar um grupo de Admin do RMS diferente no Active Directory, adicionar utilizadores e criar a lista de controlo de acesso (ACL) adequada para as páginas de administração. Por exemplo, a configuração predefinida das ACLs da página Web de administração do RMS especifica que só o utilizador que aprovisionou o servidor pode aceder à página de Definições de segurança.

<span id="BKMK_55"></span>
#### O RMS pode proteger documentos individuais assim que forem criados, no disco rígido do utilizador ou numa pasta partilhada?

Apesar de o RMS poder ser utilizado para proteger os documentos guardados no computador local de um utilizador, o Sistema de Encriptação de Ficheiros (EFS) seria a opção preferida. O EFS protege os documentos de forma transparente, enquanto que o RMS requer intervenção manual (vários cliques no rato) para proteger um documento.

<span id="BKMK_56"></span>
#### Quando abrir um ficheiro, o ficheiro de gravação automática e os ficheiros temporários estão encriptados?

Sim, todos os ficheiros temporários são encriptados.

<span id="BKMK_562"></span>
#### Quando recebo uma mensagem de correio electrónico protegida por direitos, parece que existe um anexo incluído na mensagem de correio electrónico. Posso guardar esse anexo mesmo quando não seja supostamente possível guardar o correio - o RMS é quebrado?

Não. Este é o comportamento previsto. O anexo visualizado é a mensagem encriptada antes de o cliente do RMS ter desencriptado a mensagem. Ainda está protegido por direitos e não pode ser guardado quando for desencriptado.
