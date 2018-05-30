---
TOCTitle: Plano de Recuperação do Sistema
Title: Plano de Recuperação do Sistema
ms:assetid: 'a7779ffd-7a94-4e13-b846-0ffd00608e02'
ms:contentKeyID: 18124120
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747718(v=WS.10)'
---

Plano de Recuperação do Sistema
===============================

As falhas de sistema ocorrem por diversos motivos não planeados: falhas de hardware, transbordos, picos de tensão, erros de software, etc. Uma implementação com êxito inclui planos para a recuperação rápida do sistema em caso de falha. Num sistema do RMS, o requisito primário para a protecção das capacidades do RMS é a execução regular de cópias de segurança da chave privada do servidor e das bases de dados do RMS, em especial da base de dados de configuração. Através desta prática pode preservar os modelos da política de direitos e as chaves, bem como outros dados necessários que permitem o acesso às licenças prévias e conteúdos publicados anteriormente. Se a instalação existente do RMS ficar indisponível, pode instalar o RMS noutros servidores e, em seguida, aprovisionar o RMS especificando a base de dados de configuração de cópia de segurança como a base de dados a utilizar. A nova instalação a partir dessa cópia de segurança será idêntica à da instalação anterior, na altura em que foi efectuada a cópia de segurança.

Esta secção trata de:

-   [Preparação da Recuperação do Sistema](https://technet.microsoft.com/885c047f-1e3b-4bf5-8248-3a4505759cbb)
-   [Cópias de Segurança do Sistema para o RMS](https://technet.microsoft.com/c29894da-ee00-428c-8d48-80d8e5a83678)
-   [Efectuar Cópias de Segurança e Restaurar o sistema](https://technet.microsoft.com/c11f3ac1-e512-402b-bf13-9ff21f5fe745)
-   [Efectuar Cópia de Segurança e Restaurar Modelos de Política de Direitos](https://technet.microsoft.com/a6ed3328-4128-45e8-9236-3de484b460de)
