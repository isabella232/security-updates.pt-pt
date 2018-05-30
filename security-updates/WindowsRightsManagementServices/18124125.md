---
TOCTitle: Novidades do Service Pack 2
Title: Novidades do Service Pack 2
ms:assetid: 'a944cb73-d900-42bb-b7aa-92916dead408'
ms:contentKeyID: 18124125
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747629(v=WS.10)'
---

Novidades do Service Pack 2
===========================

Os Serviços de Gestão de Direitos (RMS) com Service Pack 2 (SP2) fornecem suporte para as seguintes funcionalidades:

-   **Suporte nativo para Microsoft® SQL Server™ 2005**. Nas versões anteriores do RMS, era necessária uma solução para utilizar o RMS com o SQL Server 2005. Para obter informações sobre esta solução, consulte o artigo 913372 na Base de Dados de Conhecimento da Microsoft ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)). No RMS com SP2, este problema foi resolvido.
-   **Microsoft Office SharePoint® Server 2007**. Nesta versão, é suportado o Office SharePoint Server 2007. A biblioteca de documentos do Office SharePoint Server 2007 aplica automaticamente permissões do RMS a documentos à medida que são transferidos, com base nos direitos do Office SharePoint Server 2007. Tal é conseguido através da instalação do cliente do RMS com SP2 no servidor do Office SharePoint Server 2007. Não é recomendada a instalação do servidor do RMS com SP2 e do Office SharePoint Server 2007 no mesmo computador.
-   **Maior segurança nas mensagens para a base de dados de registo**. Nesta versão, todas as mensagens de Colocação de Mensagens em Fila dos servidores do RMS para a base de dados de registo do RMS são assinadas digitalmente.
-   **Maiores tamanhos de criação de batches em servidores**. Nesta versão, é agora possível a uma aplicação activada pelo RMS obter várias licenças de utilização para diferentes contas de utilizador a partir de um único pedido de licença ao servidor do RMS. Isto aumenta o desempenho reduzindo a sobrecarga causada por vários pedidos de licença para a mesma porção de conteúdo protegido.
-   **Melhor expansão de grupos em florestas**. Nesta versão, a expansão de grupos do RMS em florestas é feita por meio de um pedido de protocolo SOAP (Simple Object Access Protocol) a um novo serviço Web ASP.NET em execução no servidor do RMS.
