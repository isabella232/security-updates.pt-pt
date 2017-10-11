---
TOCTitle: Serviço de Escuta de Registo do RMS
Title: Serviço de Escuta de Registo do RMS
ms:assetid: 'e81ea57d-1a7d-4c02-abfc-dbc1597e176b'
ms:contentKeyID: 18124208
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747709(v=WS.10)'
---

Serviço de Escuta de Registo do RMS
===================================

O serviço de Escuta de Registo é instalado pelo programa de configuração do RMS. É executado tanto em servidores de certificações de raiz como de licenciamento. Cada serviço Web do RMS regista todos os pedidos e respostas recebidos e enviados e, em seguida, transmite os dados à fila de mensagens de registo através da Colocação de Mensagens em Fila. Em seguida, o serviço de escuta do registo transfere esses dados da fila de mensagens para a base de dados de registo do cluster respectivo.

O registo pode ser activado e desactivado a partir do Web site de Administração. Neste caso, os serviços Web deixam de efectuar o registo e desactivam o serviço de Escuta do Registo.
