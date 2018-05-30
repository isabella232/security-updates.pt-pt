---
TOCTitle: Modelos de Políticas de Direitos
Title: Modelos de Políticas de Direitos
ms:assetid: 'eee931c8-7c98-48e9-9e2c-d0b7bd4f2b96'
ms:contentKeyID: 18124227
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747732(v=WS.10)'
---

Modelos de Políticas de Direitos
================================

Os modelos de políticas de direitos descrevem um conjunto padrão de utilizadores, direitos e condições que podem ser aplicados ao conteúdo protegido pelo RMS. Quando um utilizador aplica um modelo de política de direitos a uma peça de conteúdo, os direitos nele descritos passam a fazer parte da licença de publicação. 

No Web site Administração do RMS, pode criar modelos de políticas de direitos e eliminar ou modificar modelos existentes. Os modelos de políticas de direitos podem incluir diversas condições, tais como destinatários ou grupos específicos do Active Directory, o período de validade de uma licença de utilização para o conteúdo, o período de consumo do conteúdo após a publicação e até mesmo valores personalizados para uma aplicação específica activada pelo RMS. Um modelo pode requerer uma lista de revogações. O modelo especifica o URL para o ficheiro da lista e o número de dias em que a lista é válida. Quando um destinatário pede uma licença de utilização baseada no modelo, o sistema verifica a lista de revogações antes de o utilizador poder consumir o conteúdo protegido pelo RMS. Para mais informações, consulte "[Revogação no RMS](https://technet.microsoft.com/72689f90-f3c5-4b61-94ea-d825f3199b3b)" posteriormente nesta secção.

Eis alguns exemplos de direitos que podem ser estabelecidos em modelos de política de direitos:

-   Qualquer pessoa pode ver o conteúdo, mas só o autor o pode modificar.
-   Qualquer pessoa na empresa pode ver o conteúdo, mas apenas durante um mês após a respectiva publicação.
-   Qualquer pessoa da empresa pode ver o conteúdo, mas os clientes ou outras entidades externas estão impedidas de o ver.
-   Só os destinatários especificados podem ver o conteúdo.
-   Só um destinatário especificado pode ver ou modificar o conteúdo.

Os modelos podem incluir várias condições, tais como:

-   Destinatários específicos ou grupos do Active Directory que tenham direitos sobre o conteúdo.
-   O período de validade de uma licença de utilização para o conteúdo.
-   O intervalo de tempo, após a publicação, em que o conteúdo pode ser consumido.
-   Se a licença de utilização requer ou não uma lista de revogações e a frequência de actualização da lista.
-   Os valores personalizados que são significativos para uma aplicação específica activada pelo RMS.

Os modelos de políticas de direitos são armazenados na base de dados de configuração e numa pasta partilhada. O administrador do RMS é responsável pela distribuição de modelos de políticas de direitos da pasta partilhada para os computadores clientes para que possam ser utilizados pelos autores. Para mais informações, consulte "Distribuir Modelos de Política de Direitos" em "Utilizar um Servidor do RMS" nesta colecção de documentação.

Numa aplicação activada pelo RMS, os autores podem seleccionar um modelo de política de direitos a aplicar, o qual especifica normalmente um grupo cujos membros podem consumir o conteúdo. Quando um destinatário pede uma licença de utilização, o servidor aplica o modelo de política de direitos a partir da base de dados; desta forma se assegura que os termos de uma licença de utilização reflectem sempre a versão mais actual do modelo.
