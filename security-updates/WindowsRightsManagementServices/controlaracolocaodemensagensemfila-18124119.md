---
TOCTitle: Controlar a Colocação de Mensagens em Fila
Title: Controlar a Colocação de Mensagens em Fila
ms:assetid: 'a7109399-3a84-4681-874b-f6ea1646b0a0'
ms:contentKeyID: 18124119
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747716(v=WS.10)'
---

Controlar a Colocação de Mensagens em Fila
==========================================

O registo do RMS utiliza a Colocação de Mensagens em Fila (também conhecida como MSMQ) para enviar eventos para a base de dados de registo. Cada servidor de front-end do RMS submete mensagens ao serviço Colocação de Mensagens em Fila, e o serviço de escuta do registo em cada servidor front-end obtém as mensagens de registo da fila Colocação de Mensagens em Fila e escreve-as na base de dados de registo. Se a base de dados de registo ou o servidor de base de dados ficam indisponíveis, ou se o serviço de escuta do registo for interrompido, a Colocação de Mensagens em Fila guarda as mensagens na fila. Se está a planear desligar a base de dados de registo ou o servidor de base de dados, é recomendável desligar primeiro o serviço de escuta do registo em cada um dos servidores de front-end e, em seguida, reiniciar o serviço de escuta do registo em cada um dos servidores de front-end, depois de reiniciar a base de dados ou o servidor de base de dados.

Se a base de dados falhar e o serviço de escuta do registo ainda estiver a ser executado, o serviço de escuta do registo não consegue escrever as mensagens de registo na base de dados. O serviço de escuta do registo desloca as mensagens para uma fila de Colocação de Mensagens em Fila de "mensagens não entregues" até que a base de dados fique disponível, altura em que as novas mensagens de registo serão escritas na base de dados. As mensagens na fila de mensagens não entregues não são escritas automaticamente na base de dados de registo. Para ver e apagar as mensagens na fila de mensagens não entregues, execute os seguintes passos:

1.  Abra o snap-in da Consola de Gestão da Microsoft (MMC) da Gestão de Computadores. Para tal, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Ferramentas administrativas** e clique em **Gestão de computadores**.
2.  Na árvore da consola, em Serviços e Aplicações, clique em Colocação de Mensagens em Fila e, em seguida, clique em Filas Privadas.
3.  São visíveis duas filas. O nome de ambas as filas começa por “**drms\_logging**”, seguido do nome do cluster. Uma das filas terá o nome "**drms\_logging\_***&lt;nome do cluster name&gt;***\_deadletter**". Esta é a fila das mensagens que não foram entregues. Clique no nome da fila e, em seguida, clique na fila Mensagens da fila.
4.  Faça duplo clique em cada mensagem para ver as propriedades.
5.  Para apagar a fila, clique com o botão direito do rato na fila **Mensagens da fila**, seleccione **Todas as tarefas** e, em seguida, clique em **Remover**.

Na configuração por predefinição, a Colocação de Mensagens em Fila guarda todas as mensagens em fila, até que o limite de espaço livre de armazenamento que está no servidor seja atingido. Se a Colocação de Mensagens em Fila ocupar todo o espaço livre de armazenamento, o servidor do RMS não consegue responder aos pedidos dos clientes. Para que tal não aconteça, utilize os seguintes passos para limitar a quantidade de espaço em disco que a Colocação de Mensagens em Fila pode utilizar para a colocação de mensagens em fila:

1.  Abra o snap-in da Consola de Gestão da Microsoft (MMC) da Gestão de Computadores. Para tal, clique em Iniciar, aponte para Todos os programas, aponte para Ferramentas administrativas e clique em Gestão de computadores.
2.  Na árvore da consola, em Serviços e Aplicações, clique em Colocação de Mensagens em Fila e, em seguida, clique em Filas Privadas.
3.  São visíveis duas filas. O nome de ambas as filas começa por “drms\_logging.” Execute os seguintes passos em ambas as filas:
    -   Clique em Propriedades.
    -   Seleccione a caixa de verificação Limitar armazenamento de mensagens a (KB), e introduza o tamanho total, em kilobytes, de todas as mensagens de fila que podem ser armazenadas na fila.

Se uma fila ficar cheia, as mensagens do RMS são rejeitadas, e a seguinte mensagem de evento, associada ao Event ID 48, é enviada para o registo de eventos do sistema:

"Falhou o envio do conjunto de propriedades para a Colocação de mensagens em fila."

É recomendável a configuração das ferramentas de monitorização do sistema para que possa ser alertado quando este evento ocorre, visto que significa que existe um problema com a base de dados.
