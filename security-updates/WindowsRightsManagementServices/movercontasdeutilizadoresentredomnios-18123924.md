---
TOCTitle: Mover Contas de Utilizadores entre Domínios
Title: Mover Contas de Utilizadores entre Domínios
ms:assetid: '0010b0ea-07c0-41c9-81f7-5881343d1d55'
ms:contentKeyID: 18123924
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720179(v=WS.10)'
---

Mover Contas de Utilizadores entre Domínios
===========================================

Quando configurar e aprovisionar um servidor de certificações de raiz numa organização, o servidor fica registado no Active Directory numa configuração organizada por florestas como um fornecedor de serviços do RMS. Só pode existir um cluster de certificações de raiz por floresta do Active Directory.

Em geral, quando se move uma conta de utilizador de um domínio para outro da mesma floresta, é criado um novo SID para a conta de utilizador que está no domínio novo. Em seguida, quando um utilizador tenta adquirir um novo certificado de conta de direitos a partir do servidor, o utilizador parece ser um novo utilizador para esse servidor devido ao novo SID. O servidor gera chaves novas para o utilizador e emite o novo certificado de conta de direitos utilizando o endereço de correio electrónico original do utilizador. Quando o utilizador tenta utilizar o novo certificado de conta de direitos com uma licença existente, o SID e as chaves não coincidem e o utilizador tem de adquirir uma licença nova. O mesmo é verdadeiro quando é movido para uma conta de utilizador que fica numa floresta diferente.
