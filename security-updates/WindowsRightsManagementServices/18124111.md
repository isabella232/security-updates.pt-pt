---
TOCTitle: Configurar o SMS ou a Política de Grupo para Suportar a Implementação do Cliente
Title: Configurar o SMS ou a Política de Grupo para Suportar a Implementação do Cliente
ms:assetid: '9e37c27b-8cc1-40c6-adb7-0937aa64c8db'
ms:contentKeyID: 18124111
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747703(v=WS.10)'
---

Configurar o SMS ou a Política de Grupo para Suportar a Implementação do Cliente
================================================================================

Quando implementa o RMS, tem de instalar uma aplicação activada pelo RMS nos computadores dos utilizadores, para que estes protejam e consumam conteúdo protegido pelo RMS.

Para que uma aplicação seja activada pelo RMS, tem de integrar o cliente RMS nas respectivas operações. Antes do Windows Vista®, o cliente RMS está disponível como um componente do Windows transferido separadamente a partir do Centro de Transferências da Microsoft. No entanto, se não pretender transferir o cliente separadamente para cada computador cliente da empresa, pode utilizar o Microsoft Systems Management Server (SMS), a Política de Grupo ou scripts para automatizar o fornecimento dos clientes do RMS aos computadores clientes.

| ![](/security-updates/images/Cc747703.Important(WS.10).gif)Importante                     |
|------------------------------------------------------------------------------------------------------|
| O cliente RMS está incorporado no Windows Vista. Assim, já não é necessária uma instalação separada. |

Quando utilizar o SMS para distribuir o cliente RMS, efectue o seguinte:

-   Crie um novo ficheiro de definições de pacote.
-   Extraia os ficheiros do Windows Installer a partir do ficheiro WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe. Para tal, guarde primeiro o ficheiro WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe. Não o instale. Neste exemplo, assuma que o ficheiro é guardado em c:\\nome\_pasta. Abra uma janela da linha de comandos e escreva o seguinte comando:
    `c:\folder_name\WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x/t:c:\folder_name`
    Este comando extrai os ficheiros MSDrmClient.msi e RMClientBackCompat.msi do ficheiro .exe e coloca-os em *c:\\nome\_pasta*.
-   Utilize os ficheiros do Windows Installer para a definição e origem do pacote.
-   Anuncie a disponibilidade dos pacotes na rede.

| ![](/security-updates/images/Cc747703.note(WS.10).gif)Nota                                                                                                                                    |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A instalação do software requer direitos administrativos. A política de segurança da organização pode exigir que a instalação do software do cliente RMS seja efectuada por um administrador do sistema. |

Para mais informações sobre a utilização do SMS para distribuir software, consulte o "Systems Management Server 2003 Concepts, Planning, and Deployment Guide" ([http://go.microsoft.com/fwlink/?LinkId=17401](http://go.microsoft.com/fwlink/?linkid=17401)).

Para mais informações sobre a implementação de software de cliente utilizando a Política de Grupos, consulte os tópicos sobre a implementação de software baseada na Política de Grupo ([http://go.microsoft.com/fwlink/?LinkID=38997](http://go.microsoft.com/fwlink/?linkid=38997)).
