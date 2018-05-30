---
TOCTitle: Desactivar o RMS
Title: Desactivar o RMS
ms:assetid: 'dbcacce7-434d-48a7-a11d-ef9690d78b44'
ms:contentKeyID: 18124181
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747767(v=WS.10)'
---

Desactivar o RMS
================

A desactivação corresponde ao processo de remoção do servidor do RMS e das bases de dados associadas de uma organização. Este processo permite-lhe remover o RMS da infra-estrutura sem perder acesso às informações protegidas pelo RMS. As situações expostas a seguir indicam motivos possíveis que levam uma organização a remover um servidor do RMS da infra-estrutura:

-   Migração de um servidor de prova de conceito do RMS de um ambiente piloto para o ambiente de produção.
-   Simplificação da estrutura arquitectural através da remoção e consolidação dos servidores de licenciamento no cluster raiz do RMS.
-   Intercalação dos servidores do RMS (por exemplo, resultante de uma fusão ou aquisição de empresa) através da integração de duas infra-estruturas do RMS numa só.
-   Decisão de parar de utilizar o RMS na protecção do conteúdo.

Como um servidor activo do RMS está integrado no servidor de bases de dados e no Active Directory e mantém um conjunto de conteúdo protegido por uma chave contida no servidor do RMS, a remoção do RMS da organização requer outros passos para além da simples remoção do programa do servidor. Esta secção descreve esses passos para que possa desactivar o servidor do RMS sempre que for necessário.

Esta secção trata de:

-   [Compreender o Processo de Desactivação](https://technet.microsoft.com/57bd9949-9433-437b-93ed-ffb2dff9992e)
-   [Activar o Serviço de Desactivação](https://technet.microsoft.com/45226e85-b50d-41cc-aca7-0f603f8509d5)
-   [Definir as Permissões do Directório Virtual](https://technet.microsoft.com/45112111-9608-45b1-9a86-7b313d0a1579)
-   [Remover a Protecção de Conteúdo Oferecida pelo RMS](https://technet.microsoft.com/c30361e3-50d2-4474-a87d-d38de502cf9e)
-   [Remover o Serviço Web (Desaprovisionar o RMS)](https://technet.microsoft.com/68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e)
-   [Remover Ficheiros de Programa do RMS](https://technet.microsoft.com/d1dc8a8b-f8de-487f-87b4-2174d449f0bc)
-   [Alternativas à Desactivação do RMS](https://technet.microsoft.com/4d32f35e-997d-4d10-ab66-efe217e853f7)
