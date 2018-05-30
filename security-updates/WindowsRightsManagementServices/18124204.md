---
TOCTitle: Alterar a Chave Privada do RMS
Title: Alterar a Chave Privada do RMS
ms:assetid: 'da32137e-394a-42b2-9552-ba20f4547c23'
ms:contentKeyID: 18124204
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747765(v=WS.10)'
---

Alterar a Chave Privada do RMS
==============================

Durante o aprovisionamento, o RMS cria a chave privada do RMS para o servidor. A chave privada do RMS é encriptada e armazenada na base de dados de configuração. Recomenda-se que efectue uma cópia de segurança e guarde a chave privada num local seguro. Além disso, considere utilizar um módulo de segurança por hardware para proteger a chave privada do RMS pois é utilizada no esquema de encriptação para todos os conteúdos protegidos pelo servidor do RMS. Se, por algum motivo, a chave privada do RMS ficar comprometida, tem de desaprovisionar o RMS no servidor e, em seguida, voltar a aprovisioná-lo para obter uma chave privada nova do RMS.

Se o servidor for utilizado para proteger conteúdo, todos os proprietários de conteúdo devem ser notificados e o conteúdo publicado novamente através do servidor do RMS com a nova chave privada. Quaisquer cópias do conteúdo protegido pela chave privada comprometida devem ser destruídas pois não podem ser consideradas como tendo protecção adequada.

| ![](/security-updates/images/Cc747765.Important(WS.10).gif)Importante                                                                                                                                                                                                               |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Independentemente de o servidor ter sido inscrito ou não com o Serviço de Inscrição da Microsoft, o servidor tem de repetir o processo de aprovisionamento para obter uma chave privada nova. Se tentar novamente reinscrever um servidor do RMS, a chave privada anterior do RMS é utilizada. |
