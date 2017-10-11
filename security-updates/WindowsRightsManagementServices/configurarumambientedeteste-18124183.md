---
TOCTitle: Configurar um Ambiente de Teste
Title: Configurar um Ambiente de Teste
ms:assetid: 'cdd96b05-49e2-4b6f-bfae-40b5c028ec66'
ms:contentKeyID: 18124183
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747673(v=WS.10)'
---

Configurar um Ambiente de Teste
===============================

O RMS é integrado na infra-estrutura do Active Directory e em servidores de bases de dados, tais como os que executam o Microsoft SQL Server™ 2000. Devido à natureza crítica destes componentes de suporte, deve testar exaustivamente o RMS num ambiente de teste isolado antes de o implementar na organização. Isto requer a configuração individual das instalações do Active Directory e do servidor de bases de dados no ambiente de teste.

Comece com a configuração mais básica de um servidor do RMS numa floresta com um servidor de bases de dados e um cliente. Depois de se familiarizar com o RMS, pode adaptar a configuração à topologia do ambiente de produção da organização, adicionando múltiplas florestas e acesso externo conforme as necessidades. Apesar de o ambiente de teste poder não incluir toda a redundância e as múltiplas configurações de site do plano de implementação organizacional, deve incluir, pelo menos, um servidor para cada um dos componentes de suporte que necessita implementar.

A lista seguinte descreve a configuração mínima possível para um ambiente de teste que pode utilizar para testar uma configuração básica do RMS:

-   Um controlador de domínio com o Windows 2000 Server com o Service Pack 3 (SP3) ou posterior e o SQL Server 2000 com o SP3a instalado. O SQL Server aloja as bases de dados de registo, configuração e serviços de directório do RMS. O RMS pode ser utilizado com o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A ou o SQL Server se a base de dados existir no mesmo servidor que o RMS. Se pretende utilizar um servidor remoto para suportar a base de dados, necessita do SQL Server. Pode transferir o MSDE 2000 a partir do Web site da Microsoft.

| ![](images/Cc747673.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| O Windows 2000 Server com o Service Pack 3 (SP3) é o requisito mínimo para o controlador de domínio. Recomendamos o Windows Server 2003 devido aos melhoramentos de desempenho da expansão de grupo do Active Directory. Recomendamos que o MSDE 2000 seja utilizado para suportar bases de dados do RMS apenas em ambientes de teste pois o MSDE 2000 não suporta interfaces de rede. Além disso, os termos de utilização do MSDE 2000 especificam que não é possível utilizar ferramentas de cliente de SQL Server para manipular bases de dados do MSDE 2000. Com esta restrição, não é possível ver informações de registo nem alterar dados armazenados na base de dados de configuração. |

-   Um servidor de certificações de raiz com o Windows Server 2003 no qual o RMS é instalado e aprovisionado. Se pretender, pode adicionar outros servidores para criar um cluster de certificações de raiz à medida que o teste avança.
-   Um computador cliente com o Windows XP Professional, o cliente do RMS e uma aplicação activada pelo RMS.
-   Contas de utilizadores com atributos de endereço de correio electrónico no Active Directory.

Para mais informações sobre a instalação e configuração de uma infra-estrutura básica do RMS e sobre a aplicação dos requisitos de infra-estrutura a um ambiente de produção, consulte "[Configurar uma Infra-estrutura Básica](https://technet.microsoft.com/3a0a3a47-e755-4455-bb22-0e05053723e4)" posteriormente nesta secção.
