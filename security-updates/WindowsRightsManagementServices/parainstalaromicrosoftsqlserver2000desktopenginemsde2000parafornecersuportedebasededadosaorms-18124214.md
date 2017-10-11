---
TOCTitle: 'Para Instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) para Fornecer Suporte de Base de Dados ao RMS'
Title: 'Para Instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) para Fornecer Suporte de Base de Dados ao RMS'
ms:assetid: 'c9b9cd08-98c4-424f-b3fc-d685f57c002e'
ms:contentKeyID: 18124214
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747667(v=WS.10)'
---

Para Instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) para Fornecer Suporte de Base de Dados ao RMS
==================================================================================================================

Para Instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) para Fornecer Suporte de Base de Dados ao RMS
------------------------------------------------------------------------------------------------------------------

#### Para Instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) para Fornecer Suporte de Base de Dados ao RMS

1.  Inicie a sessão utilizando uma conta de domínio que seja membro do grupo de administradores local no servidor em que pretende instalar o Microsoft SQL Server 2000 Desktop Engine (MSDE 2000).

2.  Transfira o MSDE 2000 a partir do [Web site da Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/) e guarde-o no computador.

3.  Execute o ficheiro MSDE2000A.exe para extrair o pacote de instalação do MSDE 2000 para uma pasta. Por predefinição, esta pasta terá o nome de MSDERelA, mas pode especificar um nome diferente.

4.  Abra a linha de comandos e navegue até à localização na qual guardou a instalação do MSDE 2000.

5.  Escreva o seguinte comando para instalar o Microsoft SQL Server 2000 Desktop Engine com a configuração correcta para trabalhar com o RMS, substituindo *palavra-passe* pela sua palavra-passe segura:

    **Setup.exe /i setup\\sqlrun10.msi INSTANCENAME=RMS DISABLEAGENTSTARTUP=1 SAPWD=***password*

    | ![](images/Cc747667.Important(WS.10).gif)Importante                                                                                                                                                                                                                                       |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | O serviço do MSDE deve ser iniciado depois de instalado. Pode iniciar o serviço a partir de **Serviços** no **Painel de controlo**. Recomendamos que o serviço seja configurado para iniciar automaticamente para assegurar que a base de dados do MSDE esteja sempre disponível quando o RMS estiver a ser executado. |

Não aprovisione o RMS num servidor antes de ter uma base de dados instalada para suportar a base de dados de configuração do RMS.

Recomenda-se a utilização do Microsoft SQL Server Desktop Engine para suportar as bases de dados do RMS apenas em ambientes de teste pois o Microsoft SQL Server Desktop Engine não inclui as ferramentas necessárias para o funcionamento e suporte integrais de uma base de dados empresarial. Adicionalmente, como o MSDE não suporta acesso remoto à rede, tem de instalá-lo no mesmo servidor que o RMS e não pode adicionar outros servidores do RMS ao cluster do RMS. Os termos de utilização do Microsoft SQL Server Desktop Engine especificam que não é possível utilizar ferramentas do cliente SQL Server para manipular uma base de dados do Microsoft SQL Server Desktop Engine. Esta restrição impossibilita a execução de cópias de segurança e o restauro da base de dados de configuração do RMS, a visualização das informações de registo ou a modificação directa de dados armazenados na base de dados de configuração.
