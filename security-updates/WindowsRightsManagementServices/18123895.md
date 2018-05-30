---
TOCTitle: Utilizar Contadores de Desempenho
Title: Utilizar Contadores de Desempenho
ms:assetid: '096c3b17-c082-46c4-939c-4373af0c9dec'
ms:contentKeyID: 18123895
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720180(v=WS.10)'
---

Utilizar Contadores de Desempenho
=================================

O RMS inclui vários conjuntos de objectos e contadores de desempenho que podem ser utilizados no Monitor de Sistema para controlar a actividade dos serviços do RMS. Os contadores de desempenho são específicos de cada um dos objectos de desempenho do RMS e incluem os seguintes objectos:

-   RMS: Contadores de desempenho do ActivationProxy para pedidos de activação por proxy
-   RMS: Contadores de desempenho de certificação para pedidos de certificação de contas
-   RMS: Contadores de desempenho do DirectoryServices para pesquisas no Active Directory
-   RMS: Contadores de desempenho de inscrição para pedidos de pré-inscrição
-   RMS: Contadores de desempenho de licenciamento para pedidos de publicação e de licença de utilização
-   RMS: Contadores de desempenho de registo para actividade de registo

Estes contadores de desempenho são instalados automaticamente durante o aprovisionamento, mas é necessário adicionar os contadores ao registo para iniciar o controlo.

Para adicionar um contador de desempenho:

1.  No menu **Iniciar**, aponte para **Ferramentas administrativas** e depois clique em **Desempenho**.
2.  Na caixa de diálogo **Desempenho**, clique com o botão direito do rato numa área em branco do painel dos detalhes e, em seguida, clique em **Adicionar contadores**.
3.  Na caixa de diálogo **Adicionar contadores**, na lista de objectos **Desempenho**, seleccione o contador que pretende adicionar e, em seguida, clique em **Adicionar**.

É possível utilizar as opções **Alertas e registos de desempenho** disponíveis na caixa de diálogo **Desempenho** para controlar e gerir ficheiros de registo. Para mais informações sobre cada um dos contadores de desempenho disponíveis no RMS, consulte "[Contadores do Desempenho do RMS](https://technet.microsoft.com/a2f4e30d-3c6f-4e74-bd11-8f2103f88b0c)" nesta secção. Para informações gerais sobre os contadores de desempenho, consulte a Ajuda do Monitor de Sistema.
