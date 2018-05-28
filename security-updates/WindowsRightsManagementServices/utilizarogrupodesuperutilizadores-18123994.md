---
TOCTitle: Utilizar o Grupo de Super Utilizadores
Title: Utilizar o Grupo de Super Utilizadores
ms:assetid: '0febcb3e-7124-4e51-971a-1013b928d33b'
ms:contentKeyID: 18123994
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720198(v=WS.10)'
---

Utilizar o Grupo de Super Utilizadores
======================================

Durante o aprovisionamento, o RMS cria um grupo especial de super utilizadores que tem controlo total sobre todos os conteúdos protegidos por direitos. São concedidos aos membros do grupo de super utilizadores todos os direitos de proprietário para todas as licenças de utilização emitidas pelo servidor ou cluster do RMS onde o grupo de super utilizadores está configurado. Isto significa que os membros deste grupo podem desencriptar todo e qualquer ficheiro de conteúdo protegido, bem como remover a protecção desses ficheiros. Um membro deste grupo pode, por exemplo, remover a protecção de ficheiros que foram publicados por um determinado funcionário para que um novo proprietário possa publicar e gerir os ficheiros.

O grupo de super utilizadores não tem membros por predefinição nem administradores. Quando utiliza o Web site de administração, pode especificar um grupo de segurança do Active Directory para ser utilizado como o grupo de super utilizadores do RMS. Pode utilizar um grupo Active Directory já existente ou criar um novo para este fim. O grupo deve existir na mesma floresta do Active Directory onde o RMS foi instalado. As permissões do grupo de super utilizadores são concedidas automaticamente a qualquer conta de utilizador que faça parte do grupo que especificou como sendo o grupo de super utilizadores do RMS.

Para mais informações sobre como especificar um grupo de super utilizadores para o RMS, consulte "[Para Configurar um Grupo de Super Utilizadores](https://technet.microsoft.com/f2ef847e-2824-471f-9079-5c343094aba8)" posteriormente nesta secção.

| ![](/security-updates/images/Cc720198.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                            |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Antes de designar um grupo como grupo de super utilizadores para o RMS, o grupo deve existir na mesma floresta do Active Directory onde o RMS foi instalado. As propriedades desse grupo deverão incluir um endereço de correio electrónico, incluindo um nome de domínio completamente qualificado (FQDN) igual ao nome de conta. O endereço de correio electrónico deverá ter o formato *nome\_do\_grupo*@*nome\_do\_domínio*. |
