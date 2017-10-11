---
TOCTitle: Consumir Conteúdo Protegido pelo RMS
Title: Consumir Conteúdo Protegido pelo RMS
ms:assetid: '3cf6d64b-1187-433c-bbb2-c68069bc3c30'
ms:contentKeyID: 18123979
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720251(v=WS.10)'
---

Consumir Conteúdo Protegido pelo RMS
====================================

Quando os utilizadores consomem conteúdo protegido, ocorrem dois processos, qualquer deles transparente para o utilizador. Primeiro, a aplicação activada pelo RMS pede uma licença de utilização quando o utilizador abre o documento. Em segundo lugar, a aplicação activada pelo RMS examina a licença de utilização para determinar se necessita de uma lista de revogação e verifica se algum dos certificados da respectiva cadeia de fidedignidade ou um dos certificados de contas de direitos foi revogado. Concluídos ambos os processos, a aplicação activada pelo RMS produz o conteúdo protegido pelo RMS se todos os direitos e revogações o permitirem.

Se for necessária uma lista de revogações, a aplicação procura uma cópia local da lista de revogações válida. Se necessário, obtém uma cópia actual da lista de revogações. A aplicação aplica, então, quaisquer condições de revogação relevantes ao contexto em causa.

Se não houver nenhuma revogação a bloquear o acesso ao conteúdo, a aplicação entrega o conteúdo e o utilizador pode exercer os direitos que lhe foram concedidos.

Pode configurar o RMS para processar pedidos de licença de utilização efectuados por utilizadores externos autorizados. Isto permite aos utilizadores partilharem conteúdo protegido pela Internet.

Os ficheiros de registo não são criados

-   [Aquisição da Licença de Utilização](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)
-   [Licenças de Utilização e Utilizadores Externos](https://technet.microsoft.com/02db9bda-180e-438f-863d-26252083a471)
