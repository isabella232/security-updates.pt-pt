---
TOCTitle: Avaliar Requisitos de Migração
Title: Avaliar Requisitos de Migração
ms:assetid: 'cec07f45-dc52-4004-860b-5cc33e5fc209'
ms:contentKeyID: 18124188
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747759(v=WS.10)'
---

Avaliar Requisitos de Migração
==============================

As organizações que implementam o RMS necessitam de estabelecer um plano de migração que minimize o tempo de inactividade do servidor para poderem suportar cenários de manutenção e actualização de servidores sem que tal impeça o acesso dos utilizadores a conteúdo protegido pelo RMS. Como as bases de dados de configuração e de registo anteriores podem ser utilizadas pelo RMS, a migração do RMS de um servidor para outro deve ter um impacto mínimo na organização se forem utilizados os procedimentos adequados. O cenário de migração assume que pretende utilizar as bases de dados existentes. Caso contrário, teria de efectuar uma instalação nova do RMS.

Se o servidor do RMS que está a substituir utilizar um módulo de segurança por hardware (HSM), tal como o nCipher, tem de transferir a configuração do HSM para o novo servidor antes de instalar e aprovisionar o RMS no servidor. Para obter mais instruções, consulte a documentação que acompanha o módulo de segurança por hardware.

Antes de migrar:

-   Verifique se as bases de dados estão disponíveis.
-   Decida que computadores irão ser utilizados na nova instalação.

Para migrar a instalação do RMS, utilize os seguintes passos:

1.  Efectue uma cópia de segurança de todos os componentes antes de iniciar a migração, incluindo uma cópia de segurança das bases de dados, das chaves privadas e do estado do sistema.
2.  Certifique-se de que as bases de dados da instalação anterior do RMS existem no servidor de bases de dados utilizado na nova implementação.
3.  Instale e aprovisione o RMS nos servidores apropriados, e especifique a localização das bases de dados. Tópicos relacionados

Um cenário comum que resulta na migração do servidor do RMS é a mudança de uma implementação piloto do RMS para um ambiente de produção. Para mais informações sobre este cenário de utilização, consulte "Migrar de uma Implementação Piloto do RMS para uma Implementação de Produção" em "Implementar o RMS" nesta colecção de documentação.
