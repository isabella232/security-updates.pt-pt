---
TOCTitle: Para Adicionar um Servidor a um Cluster
Title: Para Adicionar um Servidor a um Cluster
ms:assetid: 'db635238-5528-4bec-9cc6-8244e2b3d733'
ms:contentKeyID: 18124207
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747690(v=WS.10)'
---

Para Adicionar um Servidor a um Cluster
=======================================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

Em cada servidor, só pode aprovisionar o RMS num único Web site. Se desejar aprovisionar o RMS num Web site diferente do predefinido, utilize o Gestor de Serviços de Informação Internet para adicionar o Web site antes de iniciar este processo de aprovisionamento. Se o Web site que pretende aprovisionar não aparecer na lista de Web sites, feche a página **Administração Global**, adicione o Web site e, depois, inicie novamente o processo de aprovisionamento.

Se estiver a implementar o RMS num ambiente em que o nível funcional de domínio do Active Directory utiliza o modo nativo do Microsoft Windows 2000, o Windows RMS poderá não conseguir ler o atributo **memberOf** nos objectos do Active Directory quando tentar expandir os membros do grupo. Para permitir que o RMS leia o atributo **memberOf**, a conta de serviço do RMS deve utilizar uma conta de domínio que seja membro do grupo de Acesso compatível com versões anteriores ao Windows 2000 (incorporado) existente na floresta.

Adicionar um Servidor a um Cluster
----------------------------------

#### Para Adicionar um Servidor a um Cluster

1.  Depois de instalar o RMS num servidor que pretende associar a um cluster de certificações de raiz ou de licenciamentos, abra a página **Administração Global**.

2.  No Web site em que pretende aprovisionar o RMS, clique em **Adicionar este servidor a um cluster**. Pode seleccionar o Web site predefinido ou outro Web site que tenha criado nos Serviços de Informação Internet (IIS) para esse fim.

    | ![](/security-updates/images/Cc747690.Warning(WS.10).gif)Aviso                                                                                                                                                                               |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Não é suportada a execução de outros Web sites ou serviços no mesmo servidor do RMS. Se tal ocorresse, poderiam ser executados vários serviços e aplicações sob a mesma conta do RMS, o que poderia expor as chaves privadas a operações sem garantias. |

3.  Na área **Conta de serviço do RMS**, escreva o nome da conta, com o formato nome\_domínio\\nome\_utilizador, e a palavra-passe da conta de serviço do RMS com a qual o RMS será executado para a maior parte das operações normais. A conta deve ser de domínio. Todos os servidores de um cluster devem operar sob a mesma conta de serviço do RMS.

    | ![](/security-updates/images/Cc747690.Important(WS.10).gif)Importante                                                                                                                                                                                                                                       |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Por questões de segurança, é recomendável criar uma conta especial de utilizador de domínio para utilizar como conta de serviço do RMS e à qual não serão concedidas permissões especiais. A conta de serviço do RMS não pode ser a mesma conta de domínio que foi utilizada para instalar o RMS com o Service Pack 1. |

4.  Na área **Base de dados de configuração**, especifique o nome do servidor da base de dados e o nome da base de dados de configuração para esse cluster. A base de dados que seleccionar determina o cluster ao qual este servidor vai ser associado.

5.  Na área **Protecção da chave privada**, seleccione o mecanismo utilizado por este cluster para proteger a chave privada. Para a protecção predefinida de chave privada por meio de software, forneça a palavra-passe que foi utilizada para encriptar a chave privada quando o primeiro servidor desse cluster foi aprovisionado.

6.  Clique em **Submeter**.

    Se aparecerem mensagens de erro, não feche a página. Em vez disso, corrija os erros, utilize IISReset na linha de comandos para parar e reiniciar o IIS, volte à página anterior, volte a introduzir as informações de aprovisionamento e, em seguida, clique novamente em **Submeter**. Se receber um erro "Tempo limite do pedido esgotado", feche a janela, verifique se o sistema satisfaz os requisitos mínimos de hardware e tente aprovisionar novamente o servidor.
