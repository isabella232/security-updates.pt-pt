---
TOCTitle: Migrar uma Base de Dados de Configuração
Title: Migrar uma Base de Dados de Configuração
ms:assetid: '980e3e94-7d28-40dd-ad01-d34eb3c8d8e6'
ms:contentKeyID: 18124104
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747607(v=WS.10)'
---

Migrar uma Base de Dados de Configuração
========================================

Existem instâncias em que é necessário retirar um servidor de base de dados. Um exemplo é uma actualização do hardware de servidor de base de dados do RMS. Antes de retirar o servidor de base de dados, a base de dados de configuração deve ser movida para um servidor de base de dados diferente. Para proteger os dados na base de dados de configuração, incluindo os pares de chaves aí contidos, deve planear e implementar cuidadosamente uma migração.

Recomendamos a criação de um alias de CNAME para o servidor da base de dados do RMS e a configuração do RMS para utilizar este alias. Tal elimina a necessidade de alterar manualmente o nome do servidor de base de dados na base de dados de configuração do RMS se o nome do servidor for alterado. Ao utilizar um alias de CNAME, terá apenas de actualizar o registo de alias.

Antes de iniciar a migração da base de dados de configuração, certifique-se de que dispõe das seguintes informações:

-   O nome de conta e palavra-passe originalmente utilizada para aprovisionar os servidores no cluster do RMS que utilizam esta base de dados.
-   Se for utilizado um fornecedor de serviços criptográficos (CSP) baseado em software para armazenar a chave privada do RMS, a chave privada do RMS que foi originalmente especificada durante o aprovisionamento. Se for utilizado um módulo de segurança por hardware (HSM) para armazenar a palavra-passe da chave privada do RMS, este passo não é necessário.

| ![](/security-updates/images/Cc747607.note(WS.10).gif)Nota                                                                                                                                                |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A migração da base de dados de configuração não requer um novo certificado de servidor licenciador ou uma nova chave privada do servidor porque o RMS retém as definições da base de dados de configuração original. |

Antes de fazer algo no servidor de base de dados, deve efectuar uma cópia de segurança das bases de dados do RMS. Se tal não for possível deve, no mínimo, exportar o certificado de servidor licenciador. Para mais informações sobre a exportação do certificado de servidor licenciador, consulte as informações [Para Exportar o Certificado de Licenciador de Servidores para um Ficheiro](https://technet.microsoft.com/d683a629-71b3-4b11-932b-4ab0317334af). Se ocorrer um erro quando as bases de dados são migradas, pode importar o certificado de servidor licenciador para uma nova instalação do RMS e consumir conteúdo que foi protegido por direitos com a instalação antiga.

Para migrar uma base de dados de configuração, siga os seguintes passos:

-   Actualize a base de dados de configuração do RMS para reflectir o nome do novo servidor de base de dados.
-   Actualize os ficheiros web.config e o registo em cada servidor no cluster do RMS para utilizar o nome do novo servidor de base de dados

| ![](/security-updates/images/Cc747607.Important(WS.10).gif)Importante                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------|
| Este tópico presume que as bases de dados do RMS já foram copiadas para o novo servidor de base de dados que aloja as bases de dados do RMS. |

Actualize a base de dados de configuração do RMS para utilizar o nome do novo servidor de base de dados.
--------------------------------------------------------------------------------------------------------

O nome do servidor de base de dados que aloja as bases de dados do RMS é armazenado na base de dados de configuração do RMS. Após os ficheiros da base de dados serem migrados para o novo servidor de base de dados, é necessário actualizar a base de dados de configuração do RMS. Tal pode ser feito utilizando a ferramenta de Editor de Configuração do RMS, do RMS Administration Toolkit, ou utilizando o SQL Management Studio.

Para actualizar o nome de servidor de base de dados do RMS utilizando o Editor de Configuração do RMS, siga os passos seguintes:

**Para actualizar a base de dados de configuração do RMS utilizando o Editor de Configuração do RMS**
1.  Inicie sessão num servidor do RMS no cluster como membro da função de base de dados de Administradores de Sistema.

2.  Instale o RMS Administration Toolkit a partir do Centro de Transferências da Microsoft ([http://go.microsoft.com/fwlink/?LinkId=98961](http://go.microsoft.com/fwlink/?linkid=98961)).

3.  Navegue para %SystemDrive%:\\Program Files\\RMS SP2 Administration Toolkit\\RMSConfigEditor e, em seguida, faça duplo clique em **RMSCONFIGEDITOR.EXE**.

4.  Na caixa **Server**, introduza o nome do novo servidor que aloja a base de dados de configuração do RMS e, em seguida, clique na opção para avançar **Go**.

5.  Na caixa **Database**, clique em **DRMS\_Config\_***&lt;nome do cluster do RMS&gt;***\_***&lt;Porta&gt;*, em que *&lt;nome do cluster do RMS&gt;* é o nome do cluster do RMS e *&lt;Porta&gt;* é a porta TCP em que o RMS comunica e, em seguida, na opção para avançar **Go**.

6.  Clique em **DRMS\_ClusterPolicies**.

7.  No painel de resultados, altere o valor na coluna **PolicyData** da linha **LoggingDatabaseServer** para o nome do novo servidor de base de dados do RMS.

8.  Clique na opção para **Prosseguir**.

9.  Altere o valor na coluna **PolicyData** da linha **CertificationUserKeyStorageConnectionString** para reflectir o novo servidor de base de dados. O valor deve ser **data source=***&lt;nome do novo servidor de base de dados&gt;***;integrated** em que *&lt;nome do novo servidor de base de dados&gt;* é o nome do novo servidor de base de dados.

10. Clique na opção para **Prosseguir**.

11. Repita os passos 9–10 para o valor na coluna **PolicyData** da linha **DirectoryServicesCacheDatabase**.

12. No painel do lado esquerdo, clique em **DRMS\_PluginProperties**.

13. Para **PropertyID** 101, denominada **PERSISTENT\_STORAGE**, altere a coluna **PropertyValue** para reflectir o novo servidor de base de dados. O valor deve ser **data source=***&lt;nome do novo servidor de base de dados&gt;***;integrated** em que *&lt;nome do novo servidor de base de dados&gt;* é o nome do novo servidor de base de dados.

14. Clique na opção para **Prosseguir**.

15. Feche o Editor de Configuração do RMS.

Para actualizar a base de dados de configuração do RMS utilizando o SQL Server Management Studio, siga os seguintes passos:

**Para actualizar a base de dados de configuração do RMS utilizando o SQL Server Management Studio**
1.  Inicie sessão no servidor de base de dados de configuração do RMS como Administrador local ou outra conta de utilizador que seja membro do grupo de Administradores local.

2.  Clique em **Iniciar**, aponte para **Todos os Programas**, aponte para **Microsoft SQL Server 2005** e, em seguida, clique em **SQL Server Management Studio**.

3.  Na página **Ligar ao servidor**, certifique-se de que o nome do novo servidor de base de dados está listado na caixa do **Nome do servidor** e, em seguida, clique em **Ligar**.

4.  Expanda **Bases de dados**, expanda **DRMS\_Config\_***&lt;nome do cluster do RMS&gt;***\_***&lt;Porta&gt;* e, em seguida, expanda **Tabelas**.

5.  Clique com o botão direito em **DRMS\_ClusterPolicies** e, em seguida, clique em **Abrir tabela**.

6.  No painel de resultados, altere o valor na coluna **PolicyData** da linha **LoggingDatabaseServer** para o nome do novo servidor de base de dados do RMS.

7.  Altere o valor na coluna **PolicyData** da linha **CertificationUserKeyStorageConnectionString** para reflectir o novo servidor de base de dados. O valor deve ser **data source=***&lt;nome do novo servidor de base de dados&gt;***;integrated** em que *&lt;nome do novo servidor de base de dados&gt;* é o nome do novo servidor de base de dados.

8.  Repita os passos 6–7 para o valor na coluna **PolicyData** da linha **DirectoryServicesCacheDatabase**.

9.  No painel Explorador de Objectos, clique com o botão direito em **DRMS\_PluginProperties** e, em seguida, clique em **Abrir tabela**.

10. Para **PropertyID** 101, denominada **PERSISTENT\_STORAGE**, altere a coluna **PropertyValue** para reflectir o novo servidor de base de dados. O valor deve ser **data source=***&lt;nome do novo servidor de base de dados&gt;***;integrated** em que *&lt;nome do novo servidor de base de dados&gt;* é o nome do novo servidor de base de dados.

11. Feche o Microsoft SQL Server Management Studio.

Configure cada servidor no cluster do RMS para utilizar o nome do novo servidor de base de dados
------------------------------------------------------------------------------------------------

Para configurar cada servidor no cluster do RMS para utilizar o nome do novo servidor de base de dados, é necessário actualizar os ficheiros web.config e actualizar três entradas de registo. Uma vez concluída esta fase, deverá reiniciar os Serviços de Informação Internet (IIS) para que as alterações tenham efeito.

Para actualizar os ficheiros web.config em cada servidor no cluster do RMS:

**Para actualizar os ficheiros web.config em cada servidor no cluster do RMS**
1.  Inicie sessão num servidor no cluster do RMS como membro do grupo de Administradores local.

2.  Navegue para %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\admin.

3.  Faça duplo clique em **web.config**, seleccione a opção para **Seleccionar o programa de uma lista** e, em seguida, clique em **OK**.

4.  Clique em **Bloco de Notas**, desmarque a opção para **Usar sempre o programa seleccionado para abrir este tipo de ficheiro** e, em seguida, clique em **OK**.

5.  Clique em **Editar** e, em seguida, clique em **Substituir**.

6.  Na caixa **Encontrar o quê**, introduza o nome do servidor de base de dados a ser retirado que está a alojar as bases de dados do RMS.

7.  Na caixa **Substituir por**, introduza o nome do novo servidor de base de dados que está a alojar as bases de dados do RMS.

8.  Clique na opção para **Substituir tudo** e, em seguida, clique em **Cancelar**.

9.  Clique em **Ficheiro** e, em seguida, clique em **Guardar**.

10. Feche o Bloco de Notas.

11. Repita os passos 2–9 para os ficheiros web.config localizados nos directórios %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\certification e %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\licensing.

12. Repita os passos 1–11 para cada servidor no cluster do RMS.

Finalmente, actualize o registo em cada servidor no cluster do RMS para o nome do novo servidor de base de dados:

| ![](/security-updates/images/Cc747607.Caution(WS.10).gif)Atenção                                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A edição incorrecta do registo poderá danificar gravemente o sistema. Antes de efectuar alterações no registo, crie uma cópia de segurança de todos os dados importantes do computador. |

**Para actualizar o registo em cada servidor no cluster do RMS**
1.  Inicie sessão num servidor no cluster do RMS como membro do grupo de Administradores local.

2.  Clique em **Iniciar** e, em seguida, clique em **Executar**.

3.  Introduza **regedit.exe** e, em seguida, clique em **OK**.

4.  Navegue para **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\KeyProtection**.

5.  Altere a entrada de registo denominada PASSWORDDERIVEDKEY\_*&lt;nome do servidor de base de dados antigo&gt;*\_DRMS\_CONFIG\_*&lt;nome do cluster do RMS&gt;*\_*&lt;porta&gt;* para:

    PASSWORDDERIVEDKEY\_*&lt;nome do novo servidor de base de dados&gt;*\_DRMS\_CONFIG\_*&lt;nome do cluster do RMS&gt;*\_*&lt;porta&gt;*

    em que:

    -   *&lt;nome do servidor de base de dados antigo&gt;* é o nome do servidor de base de dados antigo.
    -   *&lt;nome do cluster do RMS&gt;* é o nome do cluster do RMS.
    -   *&lt;porta&gt;* é a porta TCP em que o RMS comunica.
    -   *&lt;nome do novo servidor de base de dados&gt;* é o nome do novo servidor de base de dados.

6.  Navegue para **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet001\\Services\\DRMS\_Logging\_&lt;RMS cluster name&gt;\_&lt;port&gt;\\Params**.

7.  Altere a entrada de registo **ConnectionString** de forma a que o valor de origem de dados corresponda ao nome do novo servidor de base de dados.

8.  Repita os passos 6–7 para **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\DRMS\_Logging\_&lt;RMS cluster name&gt;\_&lt;port&gt;\\Params**.

9.  Numa linha de comandos, escreva **IISRESET** e, em seguida, prima ENTER.

10. Repita os passos 1–9 para cada servidor no cluster do RMS.
