---
TOCTitle: Como Funciona a Revogação do RMS
Title: Como Funciona a Revogação do RMS
ms:assetid: '469e3938-a59b-4c92-9779-ead64e724d00'
ms:contentKeyID: 18123967
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720263(v=WS.10)'
---

Como Funciona a Revogação do RMS
================================

A revogação actua impedindo a associação, o processo que permite a um utilizador consumir conteúdo quando uma entidade revogada está envolvida no pedido de associação. A revogação é implementada através de listas de revogações distribuídas pelos computadores cliente. Essas listas são ficheiros XrML assinados que especificam o conteúdo, as aplicações, os utilizadores ou outros principais que tenham sido revogados pelo principal que emite a lista.

Cada vez que um utilizador tenta consumir conteúdo protegido, a aplicação associada activada pelo RMS envia um pedido para o direito apropriado ao cliente do RMS através de um pedido vinculativo. Por exemplo, se o utilizador tenta abrir um ficheiro, a aplicação pede direitos de Visualização para que possa abrir o ficheiro. Se o utilizador tentar editar o ficheiro, a aplicação pede direitos de Edição.

Durante o processamento do pedido vinculativo, o cliente do RMS executa os seguintes passos:

1.  Verifica se na licença de utilização existe qualquer requisito referente a uma lista de revogações.
2.  Se houver requisitos de revogação na licença de utilização, o componente cliente verifica se a lista de revogações especificada está ou não presente, e se está registada e actualizada, de acordo com o intervalo de actualização especificado na licença de utilização.
3.  Verifica se o principal que assinou a lista de revogações está especificado na licença de utilização como estando autorizado a revogar a licença.
4.  Se estas verificações forem bem sucedidas, o componente cliente determina, então, se os principais envolvidos no pedido de associação original foram ou não revogados. Se tiverem sido revogados, o pedido de associação é recusado.

As listas de revogação podem ser distribuídas aos computadores clientes pelo administrador ou podem ser transferidas para o computador por um aplicação activada pelo RMS quando forem solicitadas por uma licença de utilização. Quando uma lista de revogações é utilizada para associar uma peça de conteúdo, é registada e pode ser utilizada para associar pedidos a outras licenças de utilização, desde que a aplicação permaneça aberta. Depois de a aplicação estar fechada, a lista de revogações é desregistada.

O diagrama seguinte apresenta o processo de associação e mostra como a revogação funciona nesse processo.

![](images/Cc720263.81aa2d70-d261-49ad-b446-96a2eddba1a5(WS.10).gif)

A revogação é opcional. O administrador do RMS pode requerer a revogação, especificando-a num ou mais modelos de política de direitos da organização. Quando a revogação é requerida, uma licença não pode ser associada, a não ser que a lista de revogações requerida esteja presente e registada no computador do utilizador, e que não seja anterior ao intervalo de actualização especificado na licença de utilização.

De notar, no entanto, que a revogação pode ainda actuar sobre uma determinada licença de utilização, mesmo que esta não requeira a revogação. A revogação actua sempre que qualquer emissor de qualquer certificado existente na cadeia de fidedignidade envolvida num pedido de associação tenha emitido uma lista de revogações que esteja registada num computador cliente. Neste cenário, a lista de revogações é utilizada para processar pedidos de associação, mesmo que as licenças de utilização envolvidas não requeiram a revogação. Tal verifica-se até a aplicação activada pelo RMS ser fechada pois tal anula o registo da lista de revogações.

Por exemplo, se um utilizador tenta consumir conteúdo cuja licença de utilização emitida pela entidade A requer uma lista de revogações emitida pela entidade A, a aplicação activada pelo RMS obtém a lista de revogações através do URL especificado na licença de utilização e, em seguida, regista-a. Durante o processamento do pedido vinculativo, o cliente do RMS verifica a lista de revogações para identificar possíveis revogações.

Sem fechar a aplicação activada pelo RMS, o utilizador tenta consumir outro conteúdo cuja licença de utilização foi também emitida pela entidade A. Embora esta licença de utilização não inclua uma condição de revogação, a lista de revogações da entidade A encontra-se registada no computador do utilizador. Nesta situação, o componente cliente examina a lista de revogações antes de processar o pedido de associação.

Em seguida, o utilizador tenta consumir uma peça de conteúdo cuja licença de utilização foi emitida pela entidade C. A licença de utilização não inclui uma condição de revogação. Uma vez que a única lista de revogações que está registada no computador cliente é a lista de revogações que foi emitida pela entidade A, e esta entidade não está na cadeia de fidedignidade para a licença de utilização, nenhuma revogação é implementada na associação.

Por fim, o utilizador fecha a aplicação activada pelo RMS e volta a abrir o conteúdo que não incluía uma condição de revogação. Como a lista de revogações emitida pela entidade A foi desregistada quando a aplicação foi fechada, o cliente do RMS não a examina para processar o pedido vinculativo.
