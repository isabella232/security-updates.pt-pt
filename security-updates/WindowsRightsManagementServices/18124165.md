---
TOCTitle: Cópias de Segurança do Sistema para o RMS
Title: Cópias de Segurança do Sistema para o RMS
ms:assetid: 'c29894da-ee00-428c-8d48-80d8e5a83678'
ms:contentKeyID: 18124165
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747746(v=WS.10)'
---

Cópias de Segurança do Sistema para o RMS
=========================================

Antes de configurar a infra-estrutura e instalar o RMS, efectue uma cópia de segurança dos seguintes componentes:

-   Se utilizar uma base de dados existente do SQL Server para alojar as bases de dados de configuração e de registo, efectue uma cópia de segurança de todas as bases de dados e definições de servidor. Se estiver a actualizar uma versão anterior do RMS ou a reinstalar o RMS, certifique-se de que efectua uma cópia de segurança das bases de dados de configuração e de registo anteriores.
-   Efectue uma cópia de segurança do estado de sistema do servidor onde planeia instalar o RMS. Esta cópia de segurança armazena as chaves de registo e os valores que contêm as informações necessárias ao restauro do servidor sempre que necessário.
-   Utilize o snap-in Certificados para exportar os certificados para um ficheiro. O snap-in Certificados é também utilizado para a cópia de segurança dos dados de chave privada do RMS para um ficheiro PKCS \#12 encriptado com uma palavra-passe. Se estiver a actualizar ou a reinstalar o RMS e utilizou a encriptação predefinida baseada em software para proteger a chave privada do RMS, a chave privada foi encriptada e armazenada com a cópia de segurança da base de dados de configuração.
-   Se utilizar um módulo de segurança por hardware para tornar mais segura a chave privada, deve fazer uma cópia de segurança da configuração utilizando os métodos recomendados pelo fabricante.

Os ficheiros de cópia de segurança devem ser guardados em local seguro, juntamente com a palavra-passe utilizada para encriptar as chaves privadas.
