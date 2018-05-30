---
TOCTitle: Estimar o Crescimento da Base de Dados
Title: Estimar o Crescimento da Base de Dados
ms:assetid: '87652cc2-b886-4797-8d40-356669768089'
ms:contentKeyID: 18124082
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747585(v=WS.10)'
---

Estimar o Crescimento da Base de Dados
======================================

Quando calcular o espaço de armazenamento necessário para as bases de dados do RMS, planeie uma capacidade mínima de 10 megabytes (MB) e, em seguida, acrescente 1 MB adicional para cada 500 utilizadores da base de dados de configuração do RMS. A base de dados de registo pode existir num servidor de bases de dados diferente do utilizado para a base de dados de configuração.

Se estiver a utilizar a funcionalidade de registo do RMS, a base de dados de registo necessita de suportar um crescimento de cerca de 1 MB para cada utilizador durante a fase inicial de certificação de utilizador quando ocorre o registo em massa. Por exemplo, se a implementação suportar 1.000 utilizadores, a base de dados de registo cresce 1 gigabyte (GB) à medida que cada um destes utilizadores é activado e certificado pelo servidor de certificação do RMS. Durante as operações de rotina, a base de dados de registo pode crescer a uma velocidade de 200 kilobytes (KB) por utilizador/dia (se estiver a efectuar uma instalação faseada, estime 1 MB adicional para cada novo utilizador adicionado ao sistema).
