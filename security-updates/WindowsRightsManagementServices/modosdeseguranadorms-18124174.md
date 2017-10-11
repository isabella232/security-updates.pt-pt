---
TOCTitle: Modos de Segurança do RMS
Title: Modos de Segurança do RMS
ms:assetid: 'd7792293-5bb2-4232-9d48-e81e87ab6219'
ms:contentKeyID: 18124174
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747686(v=WS.10)'
---

Modos de Segurança do RMS
=========================

O RMS utiliza diferentes definições de segurança para os seguintes três modos:

-   Configuração: Os ficheiros do RMS são instalados e configurados.
-   Aprovisionamento: bases de dados, Web sites e directórios virtuais são criados e configurados.
-   Operações normais: Alguns serviços (tais como a certificação de contas) necessitam de ser autenticados, enquanto outros dispensam a autenticação (tais como as activações de máquinas). Enquanto alguns serviços (como a Administração) são restritos, outros (como o Licenciamento) não o são.

Em cada modo, o RMS obtém acesso a recursos diferentes para fins diferentes. Também utiliza diferentes contas de segurança, consoante as operações que tem de efectuar. Os tópicos restantes desta secção descrevem a segurança nos três modos, as operações efectuadas pelo RMS, as contas de segurança emitidas e as respectivas permissões de acesso.
