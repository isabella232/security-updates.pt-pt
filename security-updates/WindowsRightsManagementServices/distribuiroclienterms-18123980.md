---
TOCTitle: Distribuir o cliente RMS
Title: Distribuir o cliente RMS
ms:assetid: '4b8dd930-4105-4e73-918c-12d2b05d5fb5'
ms:contentKeyID: 18123980
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720266(v=WS.10)'
---

Distribuir o cliente RMS
========================

O cliente RMS está incorporado no sistema operativo Windows Vista® pelo que o cliente RMS já não constitui uma instalação separada. Os sistemas operativos anteriores ao Windows Vista obrigam a que instale o software cliente RMS e o active.

O processo de activação estabelece um cofre e um certificado de computador para o utilizador com sessão iniciada. A activação é um processo local que não requer uma ligação de rede. Quando a activação é efectuada com êxito, o primeiro pedido para uma licença de utilização por parte de uma aplicação activada pelo RMS obtém um certificado de utilizador. O cliente RMS pode ser instalado em cada computador cliente da organização utilizando a Política de Grupo, o Windows Update ou um script de administração.

| ![](/security-updates/images/Cc720266.note(WS.10).gif)Nota                                                                                                                                                                                                                                     |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Seja qual for o método de distribuição do software cliente, o cliente RMS utiliza uma porta, por predefinição a porta 80 ou 443, para comunicar com o servidor RMS. Certifique-se de que o computador cliente é capaz de efectuar pedidos de saída para a raiz e clusters apenas de licenciamento do RMS. |

**Utilizar a Política de Grupo**

Se a sua organização distribuir software utilizando uma Política de Grupo, este método pode ser utilizado para distribuir o cliente RMS utilizando privilégios elevados. Se o cliente RMS for distribuído desta forma, o utilizador não necessita de ter privilégios de administrador e pode instalar o cliente RMS utilizando **Adicionar ou Remover Programas** no **Painel de Controlo** ou abrindo conteúdo protegido pelo RMS com uma aplicação activada pelo RMS.

**Utilizar o Windows Update**

O Windows Update é a forma mais simples de instalar o cliente RMS num computador. Este método possui a vantagem de utilizar um mecanismo que é familiar aos utilizadores, mas requer que o utilizador que efectue a instalação do cliente RMS tenha direitos administrativos no computador.

**Utilizar a Instalação de Script**

Para obter o nível mais elevado de controlo sobre o processo de instalação do software cliente, pode adquirir o software e, em seguida, validar a respectiva integridade em cada fase do processo de instalação, através da execução de um script. Este script pode ser escrito e adicionado a um objecto dos Objectos de Política de Grupo (GPO) como um script de arranque. Com este método, o utilizador não tem de ser um administrador local no computador e o cliente RMS é automaticamente instalado ao reiniciar o computador.

        ```
Para mais informações básicas sobre a distribuição do cliente RMS através da Política de Grupo, consulte [Configurar o SMS ou a Política de Grupo para Suportar a Implementação do Cliente](https://technet.microsoft.com/9e37c27b-8cc1-40c6-adb7-0937aa64c8db) posteriormente nesta secção.

Para obter orientação para os processos de implementação do cliente RMS, consulte [Como Implementar o cliente RMS](https://technet.microsoft.com/c84f1724-cf71-4385-9003-ff68bc23c927) posteriormente nesta secção.
