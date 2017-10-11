---
TOCTitle: Problemas de Administração do RMS
Title: Problemas de Administração do RMS
ms:assetid: '97013c08-d3fa-4ea0-8914-995b6c97f900'
ms:contentKeyID: 18124103
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747605(v=WS.10)'
---

Problemas de Administração do RMS
=================================

Após o aprovisionamento com sucesso do RMS no servidor, podem surgir alguns problemas durante a administração quotidiana do RMS. Pode utilizar as informações fornecidas nas secções a seguir para resolver alguns destes problemas.

Mensagem "SQL Server does not exist or access denied" recebida quando tenta abrir o Web site Administração do RMS
-----------------------------------------------------------------------------------------------------------------

Se instalou o RMS utilizando uma instalação nova do SQL Server 2005 como servidor de bases de dados, o Serviço SQL Server pode não ser iniciado. No SQL Server 2005, o serviço MSSQLSERVER não está configurado para ser iniciado automaticamente quando o servidor é iniciado. Se reiniciou o SQL Server após a instalação do RMS e não configurou este serviço para ser reiniciado automaticamente, o RMS não será capaz de funcionar e só poderá aceder à página Administração Global do RMS.

Depois de iniciar o serviço MSSQLSERVER, tem de reiniciar o IIS no servidor do RMS para restaurar a funcionalidade do RMS.

Não é Possível Concluir o Processo de Inscrição Offline
-------------------------------------------------------

Se o ficheiro do pedido de inscrição estiver incompleto ou foi modificado antes de ser submetido no Web site do serviço de inscrição, não é possível concluir a inscrição offline. O ficheiro do pedido de inscrição pode ter sido danificado por um programa malicioso, erro do utilizador ou erro do sistema.

Consoante o tipo de informação em falta, o Web site do serviço de inscrição deverá aceitar o ficheiro e devolver um certificado de licenciador de servidores ou recusar-se a aceitar o ficheiro do pedido e apresentar um erro.

Se for devolvido um certificado licenciador de servidores, este reflectirá as omissões ou danos existentes no ficheiro do pedido de inscrição e o RMS apresentará um erro durante a tentativa de importação do certificado.

Se não conseguir concluir o processo de inscrição, verifique se o computador com ligação à Internet não tem vírus, reexporte o ficheiro do pedido de inscrição a partir do servidor do RMS e, em seguida, utilize um suporte diferente para o transportar para o computador com ligação à Internet. Se o erro persistir, contacte o Suporte Técnico da Microsoft.

Os Ficheiros de Registo Não São Criados
---------------------------------------

O Serviço de Registo do RMS requer o serviço Colocação de Mensagens em Fila (também conhecido por MSMQ) e acesso à base de dados de registo. Se os ficheiros de registo não estiverem a ser criados, isto pode indicar que os componentes não foram configurados correctamente ou que as comunicações entre os componentes estão a ser interrompidas.

Teste para se certificar de que o servidor do RMS e o servidor de base de dados têm ligação à rede. Se a ligação existir, utilize os procedimentos a seguir para rever os pré-requisitos do serviço de registo do RMS e certificar-se de que todas as dependências de software foram configuradas correctamente.

Em primeiro lugar, verifique se a configuração da Colocação de Mensagens em Fila está correcta. A Colocação de Mensagens em Fila deve ser instalada com a Integração com o Active Directory activada.

**Para verificar se a Colocação de Mensagens em Fila foi instalada e configurada correctamente**
1.  No **Painel de Controlo**, clique em **Adicionar ou Remover Programas** e, em seguida, clique em **Adicionar/Remover Componentes do Windows** para abrir o **Assistente de Componentes do Windows**.

2.  No **Assistente de Componentes do Windows**, seleccione a caixa de verificação **Servidor de Aplicações** e, em seguida, clique em **Detalhes**.

3.  Seleccione a caixa de verificação **Colocação de Mensagens em Fila** e, em seguida, clique em **Detalhes**.

4.  Se a caixa **Integração com o Active Directory** estiver seleccionada, vá para o teste seguinte e verifique se a Colocação de Mensagens em Fila está a funcionar. Se a caixa de verificação não estiver seleccionada, continue com os passos 5 a 9.

5.  Clique em **Iniciar**, aponte para **Todos os Programas**, aponte para **Windows RMS** e, em seguida, clique em **Administração do Windows RMS** para abrir a página Administração Global.

6.  Ao lado do Web site em que o RMS está aprovisionado, clique em **Remover o RMS deste Web site** e, em seguida, clique em **OK**.

7.  Em **Adicionar ou Remover Programas** no **Painel de Controlo**, clique em **Adicionar/Remover Componentes do Windows**, clique em **Servidor de Aplicações** e, em seguida, clique em **Colocação de Mensagens em Fila**.

8.  Para activar a **Integração com o Active Directory**, clique em **Detalhes**, seleccione a caixa de verificação **Integração com o Active Directory** e, em seguida, clique em **OK**.

9.  Abra a **página Administração Global**. Ao lado do nome do Web site no qual pretende aprovisionar o RMS, clique em **Aprovisionar o RMS neste Web site**.

Em segundo lugar, verifique se a Colocação de Mensagens em Fila está a funcionar no servidor.

**Para verificar se a Colocação de Mensagens em Fila está a funcionar no servidor**
1.  No **Painel de Controlo**, clique em **Ferramentas Administrativas** e, em seguida, clique em **Serviços**.

2.  Percorra a lista de serviços até localizar o serviço **Colocação de Mensagens em Fila**.

3.  Na coluna **Estado**, o serviço deve apresentar **Iniciado**. Se não for o caso, clique com o botão direito do rato no serviço e, em seguida, clique em **Iniciar**.

Em terceiro lugar, verifique se o serviço de registo tem permissão para escrever eventos na base de dados de registo. O serviço de registo do RMS é executado através da conta de serviço do RMS. Verifique se a conta de serviço do RMS tem um início de sessão válido no servidor de bases de dados e se lhe foram concedidas as permissões necessárias para criar bases de dados e escrever informações nos ficheiros.

Depois de todos estes pré-requisitos terem sido satisfeitos, pare e reinicie o serviço de registo do RMS utilizando o snap-in Serviços. Após o reinício do serviço de registo do RMS, os ficheiros de registo devem ser criados no servidor de bases de dados. Se estiver a utilizar o SQL Server como servidor de bases de dados, o procedimento a seguir indica como pode verificar se os ficheiros de registo estão a ser criados.

**Para verificar se os ficheiros de registo estão a ser criados no SQL Server**
1.  No SQL Server Enterprise Manager, vá para a base de dados de registo, expanda **Databases** e, em seguida, expanda a base de dados que contém a base de dados de registo do RMS.

2.  Clique na base de dados de registo, clique em **Tables**, clique com o botão direito do rato em **DRMS\_log\_master** e, em seguida, clique em **Open table – return all rows**. Se os ficheiros de registo estiverem a ser criados, é possível ver um ou mais ficheiros de registo.

Restaurar a Base de Dados de Configuração
-----------------------------------------

O RMS não pode ser utilizado sem uma base de dados de configuração que funcione correctamente. Se tiver problemas com a base de dados de configuração, como, por exemplo, a danificação da base de dados ou a falha do disco rígido do servidor de base de dados, pode restaurar a funcionalidade do RMS através do restauro de uma cópia de segurança da base de dados de configuração. Para restaurar a base de dados de configuração do RMS a partir de uma cópia de segurança, necessita das seguintes informações:

-   O nome da cópia de segurança mais recente da base de dados.
-   O nome do computador no qual a base de dados de cópia de segurança será restaurada.
-   O nome e a palavra-passe da conta originalmente utilizada no aprovisionamento do RMS.
-   A palavra-passe originalmente especificada para a protecção da chave privada (se existente) do software.

O restauro a partir da base de dados de cópia de segurança não requer um certificado de licenciador de servidores novo nem uma chave privada nova pois o RMS retém estas definições (obtendo-as a partir da base de dados de configuração de cópia de segurança).

Pode restaurar uma base de dados de cópia de segurança utilizando o procedimento descrito a seguir.

**Para restaurar uma base de dados de cópia de segurança**
1.  Clique em **Iniciar**, aponte para **Todos os Programas**, aponte para **Windows RMS** e, em seguida, clique em **Administração do Windows RMS** para abrir a página **Administração Global**.

2.  Ao lado do Web site no qual o RMS está aprovisionado, clique em **Remover o RMS deste Web site** e, em seguida, clique em **OK**.

3.  Restaure os ficheiros da base de dados de cópia de segurança para a base de dados de configuração. Se efectuou uma cópia de segurança da base de dados de registo durante o procedimento de cópia de segurança e pretende manter a continuidade dos dados, restaure também a base de dados de registo.

    -   Se este sistema estiver a ser restaurado após uma falha total do sistema, restaure o registo utilizando a cópia de segurança de estado do sistema antes de restaurar os ficheiros da base de dados.

4.  Se a base de dados a restaurar se destinar a um servidor de certificação de raiz único, modifique a seguinte chave do registo antes de tentar reaprovisionar o serviço:

    -   Em computadores com a versão de 32 bits do Windows Server 2003:
        `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0\`
    -   Em computadores com a versão de 64 bits do Windows Server 2003:
        `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0\`

    Adicione a seguinte entrada como um valor de cadeia e deixe o valor em branco:

    `GicURL`

    Isto anula a detecção do servidor de certificação de raiz pelo Active Directory, permitindo o acesso às páginas de aprovisionamento do servidor de certificação de raiz.

5.  Se utilizou um módulo de segurança por hardware para proteger a chave privada do RMS, restaure a localização de segurança de cópia de segurança para que as chaves possam ser obtidas.

6.  Utilize um dos seguintes passos:

    -   Para restaurar a base de dados para um só servidor e não para um cluster, clique em Aprovisionar o RMS neste Web site junto do Web site no qual pretende aprovisionar o RMS.
        - ou -
    -   Para restaurar a base de dados para um cluster, clique em Adicionar este servidor a um cluster junto do Web site no qual pretende aprovisionar o RMS.

7.  Especifique a conta de serviço do RMS que foi utilizada para aprovisionar o servidor originalmente.

8.  Especifique a base de dados de configuração de cópia de segurança (incluindo o nome da base de dados e o nome do computador onde a base de dados reside) que pretende utilizar.

9.  Especifique a mesma palavra-passe utilizada para aprovisionar este servidor originalmente.

10. Clique em **Submeter**.

O processo de aprovisionamento é iniciado e o RMS é reaprovisionado no servidor.

Para mais informações, consulte Plano de Recuperação do Sistema e Efectuar Cópias de Segurança e Restaurar o Sistema para o RMS em Planear uma Implementação do RMS nesta recolha de documentação.

Palavra-passe da Conta de Serviço do RMS Expirada
-------------------------------------------------

Se o RMS deixar de funcionar, a palavra-passe da conta de serviço do RMS pode ter expirado. Veja no Gestor do IIS. Se os conjuntos de aplicações do RMS pararem e não conseguir reiniciá-los, a palavra-passe da conta de serviço do RMS pode ter expirado.

Se a palavra-passe da conta de serviço do RMS expirar, tem de alterar a palavra-passe em cada servidor do RMS que utilize a conta com a palavra-passe expirada e, em seguida, reiniciar o IIS. Para mais informações, consulte "Alterar a Palavra-passe da Conta de Serviço do RMS" em "Utilizar um Servidor do RMS" nesta colecção de documentação.

Restaurar uma Instalação Anterior do RMS
----------------------------------------

Se ocorrer uma falha de hardware ou software no servidor do RMS, pode restaurar um servidor do RMS utilizando a base de dados de configuração anteriormente instalada para aprovisionar uma nova instância do servidor.

| ![](images/Cc747605.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Este procedimento só se aplica se ocorrer uma falha no servidor no qual o RMS está a ser executado. Se ocorrer uma falha no servidor que está a executar a base de dados de configuração, consulte "Restaurar a Base de Dados de Configuração" anteriormente nesta secção. Se o servidor do RMS for também o servidor de bases de dados, tem de restaurar todo o servidor a partir de uma cópia de segurança. |

Utilize o procedimento seguinte para especificar a mesma base de dados de configuração que foi utilizada na instalação original.

**Para restaurar uma instalação anterior do RMS**
1.  Inicie sessão no computador que pretende configurar como servidor do RMS utilizando uma conta com privilégios administrativos. Certifique-se de que este computador cumpre os requisitos de sistema mínimos para o RMS. Para mais informações sobre os requisitos de sistema do RMS, consulte "Requisitos de Hardware" para o RMS em "Planear uma Implementação do RMS" nesta colecção de documentação.

2.  Se estiver a utilizar um módulo de segurança por hardware para proteger as chaves privadas do RMS, certifique-se de que o módulo está configurado correctamente utilizando a definição e a localização de segurança especificadas na instalação anterior do RMS.

3.  Instale o RMS no computador.

4.  Após concluir a instalação do RMS, clique em **Iniciar**, aponte para **Todos os Programas**, aponte para **Windows RMS** e, em seguida, clique em **Administração do Windows RMS** para abrir a página **Administração Global**.

5.  Ao lado do Web site no qual pretende aprovisionar o RMS, clique em **Adicionar este servidor a um cluster**.

6.  Na área **Conta de serviço do RMS**, escreva o nome da conta de serviço do RMS utilizando o formato nome\_domínio\\nome\_utilizador e a palavra-passe da conta de serviço do RMS na qual o RMS será executado para a maior parte das operações de rotina. A conta deve ser de domínio.

7.  Na área **Base de dados de configuração**, especifique o nome do servidor de bases de dados e o nome da base de dados de configuração da instalação original do RMS que pretende recuperar.

8.  Na área **Protecção da chave privada**, seleccione o mecanismo utilizado por este cluster para proteger a chave privada. Se tiver sido utilizada a protecção de chave privada baseada no software, é necessário fornecer a palavra-passe utilizada para encriptar a chave privada quando este cluster foi aprovisionado originalmente.

9.  Clique em **Submeter**.

Os clientes não conseguem abrir conteúdo protegido pelo RMS devido a permissões expiradas
-----------------------------------------------------------------------------------------

Se as permissões de um utilizador expirarem, o utilizador não consegue consumir conteúdo protegido pelo RMS. Se o relógio de sistema do servidor do RMS estiver adiantado em relação ao relógio de sistema do cliente do RMS, o utilizador pode também não conseguir consumir conteúdo protegido pelo RMS mesmo que as permissões não tenham expirado. Como o relógio de sistema dos dois componentes não está sincronizado, o erro indicado a seguir pode ser apresentado quando o computador cliente tenta abrir o conteúdo:

**Não tem permissão para abrir esta mensagem porque a permissão expirou. Pretende abri-la utilizando um conjunto de credenciais diferente?**

Tanto a licença do cliente como a licença de conteúdo são válidas, mas a diferença temporal faz com que o cliente interprete a licença de conteúdo como sendo inválida e devolva este erro ao utilizador. Isto pode levar o utilizador a pensar que existe um problema com o certificado de conta do RMS ou com os direitos concedidos ao documento. Assim que o relógio do cliente atinge o intervalo de tempo de validade da licença de publicação de conteúdo, o utilizador consegue abrir o conteúdo.

Como procedimento recomendado, os clientes e os servidores do sistema do RMS devem ser sincronizados para o mesmo serviço de hora.

Erro "O Acesso É Negado" quando o RMS Tenta Registar Eventos no Registo de Eventos da Aplicação
-----------------------------------------------------------------------------------------------

Por predefinição, os componentes que são executados a partir de uma página ASP, como o RMS, são criados na conta IUSR\_COMPUTERNAME. Esta conta é um membro do grupo Convidados e os privilégios de segurança que permitem escrever no registo de eventos da aplicação impedem as contas de Convidados de escreverem dados no registo de eventos.

Para resolver este problema, pode utilizar o editor de registo para modificar a chave de registo que controla este comportamento.

| ![](images/Cc747605.Caution(WS.10).gif)Atenção                                                                                                                    |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Uma edição incorrecta do registo pode danificar gravemente o sistema. Antes de proceder a alterações do registo, efectue uma cópia de segurança dos dados importantes guardados no computador. |

Defina a chave de registo indicada a seguir como 0 e não como 1. Em seguida, reinicie o computador para implementar as alterações.

`HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\EventLog\Application`

Nome: `RestrictGuestAccess`

Tipo: `REG_DWORD`

| ![](images/Cc747605.note(WS.10).gif)Nota                       |
|---------------------------------------------------------------------------------------------|
| Isto permite que todas as contas de Convidados escrevam no Registo de Eventos da Aplicação. |

Para mais informações sobre a causa deste erro, consulte o artigo sobre como activar o registo a partir de páginas ASP na [Base de Dados de Conhecimento](http://go.microsoft.com/fwlink/?linkid=44167).
