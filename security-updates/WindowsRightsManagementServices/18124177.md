---
TOCTitle: Para Importar e Utilizar o RMS Management Pack
Title: Para Importar e Utilizar o RMS Management Pack
ms:assetid: 'd9a73ef0-2f81-48c2-97cc-deb7bf477389'
ms:contentKeyID: 18124177
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747688(v=WS.10)'
---

Para Importar e Utilizar o RMS Management Pack
==============================================

Importar e Utilizar o RMS Management Pack
-----------------------------------------

#### Para Importar e Utilizar o RMS Management Pack

1.  Copie o pacote de gestão RMS (RMS\_MOMPack.akm) a partir da pasta %ProgramFiles%\\Windows Rights Management Services\\Tools para o servidor Microsoft Operations Manager (MOM).

2.  Abra a consola do administrador do MOM e, em seguida, importe o pacote de gestão RMS utilizando os seguintes passos:

    1.  Na árvore da consola do administrador do MOM, expanda o item **Rules** e, em seguida, clique com o botão direito do rato no item **Processing Rule Groups**.
    2.  No menu de atalho, clique em **Import Management Pack**. É apresentada a caixa de diálogo **Import Management Pack**.
    3.  Clique em **Browse** e, em seguida, seleccione o ficheiro RMS\_MOMPack.akm.

3.  Especifique as opções de intercalação ou de substituição. Para mais informações sobre as opções de intercalação e substituição, consulte "Exporting and Importing Management Packs" no Web site da Microsoft (http://www.microsoft.com/).

    Clique em **Replace**. Com a opção de substituição, o pacote de gestão importado substitui os grupos de regras de processamento existentes; os comentários dos utilizadores não são preservados. Se desejar intercalar este pacote de gestão com um existente, deverá fazê-lo num ambiente de teste e, em seguida, utilizar a opção **Replace** quando implementar o pacote de gestão no ambiente de produção.

4.  Clique em **Import**, para importar o pacote de gestão.

5.  Na consola **MOM Administrator**, seleccione o item **Configuration** e, em seguida, clique na pasta **Agent Managers**.

6.  Clique com o botão direito do rato no nome do servidor para o qual importou o RMS Management Pack e, em seguida, clique em **Scan Managed Computers Now**.
