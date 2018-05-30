---
TOCTitle: Proteger as Bases de Dados Utilizadas pelo RMS
Title: Proteger as Bases de Dados Utilizadas pelo RMS
ms:assetid: '65802f9a-81bc-4398-968a-00c9b1dca2fa'
ms:contentKeyID: 18124010
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720285(v=WS.10)'
---

Proteger as Bases de Dados Utilizadas pelo RMS
==============================================

O RMS cria e utiliza três bases de dados, as quais têm diferentes requisitos de segurança, conforme indicado em seguida:

-   **Serviços de directório**. Esta base de dados guarda em cache os resultados das pesquisas dos membros do grupo Active Directory. Dado que contém apenas informação do Active Directory, não requer nenhuma segurança adicional para além da que é configurada automaticamente durante o aprovisionamento do RMS.
-   **Registo**. A informação contida nesta base de dados é mais sensível do que a que está na base de dados de serviços de directório porque a sua divulgação poderá afectar a privacidade dos utilizadores. A Microsoft teve cuidados redobrados para se assegurar de que nenhumas informações de identificação pessoal (PII) fiquem registadas e que todas as informações registadas nesta base de dados estejam protegidas através de medidas de segurança apropriadas. Não são necessárias alterações de segurança nesta base de dados, a não ser que a base de dados seja mudada para outro SQL Server. Se a base de dados for mudada para outro servidor, deverá certificar-se de que são aplicados ao novo ambiente os mesmos mecanismos de protecção.
-   **Configuração**. Para além do servidor de chaves privadas, esta base de dados é o recurso mais importante e valioso da sua implementação de RMS. Contém informações sensíveis e cruciais que deverão ser cuidadosamente protegidas. Contém todos os certificados e chaves, a chave privada do servidor encriptado (salvo se utilizou a encriptação por hardware recomendada) e o "hash" da palavra-passe da chave privada, para além das informações de configuração.

Quando o RMS cria as bases de dados de configuração, define permissões que restringem o acesso e ajudam a assegurar a segurança da sua base de dados.

Aumentar a Segurança das Bases de Dados
---------------------------------------

Pode utilizar os seguintes passos adicionais para aumentar a segurança geral das bases de dados integradas na rede e no ambiente de servidores:

-   Execute o servidor de base de dados num computador com o Windows Server 2003. Por predefinição, este sistema operativo é mais seguro do que o Windows 2000 Server. Apesar de poder bloquear um computador com o Windows 2000 Server, será uma tarefa morosa e poderá cometer erros que podem dar aos hackers uma forma de acesso à base de dados.
-   Restringir o acesso ao servidor de base de dados. Coloque o servidor numa localização que seja fisicamente segura.
-   Certifique-se de que as permissões da base de dados e as listas de controlo de acesso discricionário (DACLs) que estão nos ficheiros da base de dados restringem o acesso a pessoas autorizadas. As permissões predefinidas e as DACLs configuradas pelo RMS são seguras. Seja cuidadoso ao alterar qualquer uma das predefinições.
-   Não execute nenhum serviço desnecessário no servidor das bases de dados, como, por exemplo, os Serviços de Informação Internet (IIS) da Microsoft, a Colocação de Mensagens em Fila ou os Serviços de Terminal.
-   Não execute quaisquer bases de dados no servidor de base de dados, à excepção das bases de dados do RMS.

Proteja as bases de dados do SQL Server configurando o Secure Sockets Layer (SSL) ou o Internet Protocol Security (IPSec) para disponibilizar canais encriptados. A encriptação das comunicações das bases de dados ajudam a evitar que utilizadores com intenções dolosas capturem ou modifiquem dados registados.

Para mais informações acerca da configuração do SSL para o SQL Server 2000, consulte o [Web site da MSDN http://www.microsoft.com/](http://www.microsoft.com/) (http://www.microsoft.com/).

Para mais informações acerca da configuração do IPsec para o SQL Server 2000, consulte o [Web site da MSDN http://www.microsoft.com/](http://www.microsoft.com/) (http://www.microsoft.com/).

Para mais informações sobre como proteger o SQL Server, consulte o [Web site da Microsoft http://www.microsoft.com/](http://www.microsoft.com/) (http://www.microsoft.com/).

Também pode transferir mais documentação sobre como proteger o Windows Server 2003 a partir do [Centro de Transferências da Microsoft http://go.microsoft.com/fwlink/?LinkID=5317](http://go.microsoft.com/fwlink/?linkid=5317).
