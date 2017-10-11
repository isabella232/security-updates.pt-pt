---
TOCTitle: Implementar Listas de Revogações
Title: Implementar Listas de Revogações
ms:assetid: 'e331338b-66d4-45e4-8d3f-acccf2302ac4'
ms:contentKeyID: 18124223
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747702(v=WS.10)'
---

Implementar Listas de Revogações
================================

Para implementar uma revogação, é necessário implementar listas de revogações. As listas de revogações especificam o conteúdo, as aplicações, os utilizadores ou outros principais que tenham sido revogados. É possível implementar listas de revogações de organizações e listas de revogações da Microsoft.

Implementar Listas de Revogações de Organizações
------------------------------------------------

Para utilizar um modelo de política de direitos com uma lista de revogações, é necessário colocar a lista à disposição dos computadores cliente que se encontram na organização. Para mais informações sobre a criação de listas de revogações, consulte "Implementar uma Revogação" anteriormente nesta secção.

Pode implementar uma lista de revogações de uma organização utilizando os seguintes passos:

1.  Copie o ficheiro da lista de revogações para um servidor de Web com acesso público. Como os utilizadores podem consumir o conteúdo protegido fora da organização, o local especificado deverá ser acessível a todos os utilizadores, tanto dentro como fora da rede.
    A distribuição do ficheiro da lista de revogações a computadores cliente pode demorar algum tempo. Por isso, existe a possibilidade de os utilizadores não terem a lista de revogações disponível nos seus computadores cliente quando tentarem abrir um documento que requeira uma lista de revogações. Se a lista de revogações não se encontrar no computador cliente, a aplicação activada pelo RMS poderá transferi-la a partir da localização especificada na licença de utilização.
    O ideal seria criar um script que assinasse e copiasse automaticamente a lista de revogações para o Web site todos os dias. Isto ajudaria a garantir que os utilizadores não eram impedidos de consumir conteúdos por terem uma lista de revogações desactualizada. Para obter um script de exemplo, consulte "Utilizar a Ferramenta de Assinatura da Lista de Revogações" anteriormente nesta secção.
2.  No modelos de política de direitos, especifique um intervalo de actualização superior a zero para a lista de revogações da organização. Desta forma, garante-se que a lista de revogações não é opcional. Se a lista for actualizada com pouca frequência, por exemplo, apenas no caso de ocorrer uma quebra da segurança, pode definir um intervalo de tempo longo para a condição de actualização, e depois dependerá das definições do script ou da política enviar a lista de revogações para os computadores cliente sempre que necessário. Para mais informações sobre a definição de intervalos de actualização, consulte "Definir Políticas de Revogação" anteriormente nesta secção. Para mais informações sobre a configuração de modelos de política de direitos, consulte "Criar e Modificar Modelos de Política de Direitos" posteriormente nesta secção.
3.  No modelo de política de direitos, especifique o URL em que a lista de revogação está disponível.
4.  Opcionalmente, implemente a lista de revogações nos computadores cliente utilizando um método automático, como a Política de Grupo ou o SMS (Systems Management Server).

Implementar Listas de Revogações da Microsoft
---------------------------------------------

Para o cliente dos Serviços de Gestão de Direitos utilizar uma lista de revogações da Microsoft, é necessário implementar a lista nos computadores cliente. Este tópico descreve a forma como se pode implementar uma lista de revogações da Microsoft nos seguintes cenários:

-   A organização pretende implementar a sua própria lista de revogações e a lista de revogações da Microsoft.
-   A organização pretende implementar apenas a lista de revogações da Microsoft.

Quando a Microsoft publicar uma lista de revogações, pode transferi-la a partir dos seguintes locais:

-   Os servidores do RMS serão capazes de transferir a lista de revogação através do Windows Update.
-   Em alternativa, a lista de revogação da Microsoft estará também disponível no Centro de Transferências da Microsoft, se o servidor do RMS não estiver ligado à Internet.

Se transferir o pacote da lista de revogações para um servidor do RMS, o pacote é guardado na pasta %systemdrive%\\Program Files\\Windows Rights Management Services Revocation List. Se estiver a transferir o pacote de listas de revogações para outro tipo de computador, pode seleccionar o local da transferência. O pacote contém um ficheiro executável, CRL\_Update.exe, que pode ser executado para instalar todas as listas de revogações de clientes no arquivo das licenças do cliente e também um ficheiro de lista de revogações, Msrl.xml, que pode ser copiado para um Web site ou uma pasta partilhada.

**Para implementar a lista de revogações de uma organização e uma lista de revogações da Microsoft**
1.  Para implementar a lista de revogações da organização, siga as instruções de "[Implementar Listas de Revogações](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)" anteriormente nesta secção.

2.  Transfira o pacote da lista de revogações da Microsoft e implemente-o em todos os computadores cliente da organização utilizando um método como a Política de Grupo ou o SMS (Systems Management Server). Em alternativa, pode copiar entradas da lista de revogações da Microsoft para a lista de revogações da organização e implementar apenas a lista de revogações da organização.

| ![](images/Cc747702.Caution(WS.10).gif)Atenção                                                                                                                                                                                                                                                                                                                                                                                                    |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A Microsoft é um principal na cadeia de fidedignidade de todos os certificados e licenças que são emitidos pelo RMS. Por conseguinte, uma lista de revogações que seja emitida pela Microsoft entra em vigor para todos os pedidos de associação para os quais a licença de utilização é obtida com base num modelo de política de direitos que requer a lista de revogações da organização. Além disso, a lista de revogações da Microsoft é registada no computador cliente. |

**Para implementar apenas uma lista de revogações da Microsoft**
1.  Transfira o pacote da lista de revogações da Microsoft.

2.  Modifique os modelos de políticas de direitos existentes de forma a requererem revogação ou, no caso de não existirem modelos de política de direitos, crie um que requeira revogação. Utilize a chave pública da Microsoft quando especificar a condição de revogação.

3.  O intervalo de actualização deverá ter um valor bastante elevado, por exemplo 50.000. Este número elevado garantirá que uma lista de revogações publicada pela Microsoft nunca expira. Por conseguinte, as licenças de utilização distribuídas por si não irão requerer uma nova versão da lista de revogações da Microsoft quando não puder estar disponível uma lista.

4.  Copie o ficheiro da lista de revogações para um servidor de Web com acesso público. Como os utilizadores podem consumir o conteúdo protegido fora da organização, o local especificado deverá ser acessível a todos os utilizadores, tanto dentro como fora da rede.

5.  Tem de disponibilizar a lista de revogações, porque a distribuição do ficheiro da lista de revogações pelos computadores cliente pode levar algum tempo. Existe, por isso, a possibilidade de um utilizador não ter a lista de revogações disponível localmente no seu computador quando tentar abrir um documento com uma licença de publicação que requeira uma lista de revogações. Se a lista de revogações não estiver presente no computador cliente, a aplicação activada pelo RMS poderá transferi-la do local especificado.

6.  No modelo de política de direitos, especifique o URL em que a lista de revogação está disponível. Para mais informações sobre a configuração de modelos de política de direitos, consulte "[Criar e Modificar Modelos de Política de Direitos](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" posteriormente nesta secção.

7.  Opcionalmente, implemente o pacote da lista de revogações nos computadores cliente utilizando um método, como o método de Política de Grupo ou de SMS. Os utilizadores poderão então abrir o conteúdo protegido pelo RMS que requeira listas de revogações, mesmo que não estejam ligados à rede.
