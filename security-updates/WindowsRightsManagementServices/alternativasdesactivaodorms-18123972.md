---
TOCTitle: Alternativas à Desactivação do RMS
Title: Alternativas à Desactivação do RMS
ms:assetid: '4d32f35e-997d-4d10-ab66-efe217e853f7'
ms:contentKeyID: 18123972
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720268(v=WS.10)'
---

Alternativas à Desactivação do RMS
==================================

Se ainda planeia utilizar o RMS na organização mas, por algum motivo, pretende não utilizar determinados servidores do RMS, considere recorrer às seguintes alternativas à desactivação.

**Configurar um domínio de publicação fidedigno**

Todas as informações protegidas pelo RMS são encriptadas pela chave privada do servidor do RMS. Um domínio de publicação fidedigno permite-lhe importar a chave privada de um servidor do RMS para outro servidor do RMS. Assim, o servidor do RMS fica apto a emitir licenças de utilização associadas às licenças de publicação criadas por um servidor diferente do RMS. Após a exportação da chave, o servidor pode ser desaprovisionado e desinstalado.

**Configurar um grupo de super utilizadores**

Se não for possível abrir o conteúdo protegido pelo RMS porque nenhum dos utilizadores tem direitos para o conteúdo, pode conceder controlo total ao grupo de super utilizadores para todo o conteúdo protegido pelo RMS publicado por esse servidor. São concedidos aos membros do grupo de super utilizadores todos os direitos de proprietário para todas as licenças de utilização emitidas pelo servidor ou cluster do RMS onde o grupo de super utilizadores está configurado. Isto significa que os membros deste grupo podem desencriptar todo e qualquer ficheiro de conteúdo protegido, bem como remover a respectiva protecção. Um membro deste grupo pode, por exemplo, remover a protecção de ficheiros publicados por um determinado funcionário para que um novo proprietário possa publicar e gerir os ficheiros.

O grupo de super utilizadores não inclui automaticamente quaisquer membros, nem mesmo administradores. Este grupo tem de existir no Active Directory como grupo de distribuição com um atributo de endereço de correio electrónico com um valor igual ao do nome de grupo e com o formato "*nome\_grupo*@*nome\_domínio*.com." O nome do grupo tem de ser igual ao atributo de endereço de correio electrónico e é sensível a maiúsculas e minúsculas.
