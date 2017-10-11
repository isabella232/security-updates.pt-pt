---
TOCTitle: Base de Dados de Configuração do RMS
Title: Base de Dados de Configuração do RMS
ms:assetid: '769adbdc-f32f-464b-85c4-e8b160036187'
ms:contentKeyID: 18124051
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747634(v=WS.10)'
---

Base de Dados de Configuração do RMS
====================================

O RMS utiliza um servidor de bases de dados, como o Microsoft® SQL Server ou o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A, para armazenar as informações de configuração e políticas. Existe uma base de dados de configuração para cada servidor ou cluster do RMS. Esta base de dados armazena, partilha e obtém dados de configuração e outros.

A base de dados de configuração do servidor ou cluster de certificações de raiz contém uma lista de identidades de utilizadores do Windows e dos respectivos certificados de contas de direitos. O par de chaves de certificados é encriptado para a chave pública do servidor do RMS armazenada na base de dados. As bases de dados de configuração dos servidores de licenciamentos não contêm estas informações.

O RMS Service Group possui permissões de Execução nos procedimentos armazenados da base de dados.

**Importante   **Recomendamos que o MSDE 2000 seja utilizado para suportar bases de dados do RMS apenas em ambientes de teste pois o MSDE 2000 não suporta interfaces de rede. Além disso, os termos de utilização do MSDE 2000 especificam que não é possível utilizar as ferramentas de cliente do SQL Server para manipular bases de dados do MSDE 2000. Com esta restrição não é possível ver informações relativas ao registo nem alterar dados armazenados na base de dados de configuração.
