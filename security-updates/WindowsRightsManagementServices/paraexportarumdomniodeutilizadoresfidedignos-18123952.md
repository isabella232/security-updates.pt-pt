---
TOCTitle: Para Exportar um Domínio de Utilizadores fidedignos
Title: Para Exportar um Domínio de Utilizadores fidedignos
ms:assetid: '40281ba3-2674-43ca-aa6d-1deb9302eb0e'
ms:contentKeyID: 18123952
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720259(v=WS.10)'
---

Para Exportar um Domínio de Utilizadores fidedignos
===================================================

Para efectuar este procedimento, tem de iniciar sessão localmente no Web site Administração com uma conta de utilizador de domínio que seja membro do grupo Administradores no computador a que está a aceder. Os membros do grupo de administradores de domínio também podem efectuar este procedimento. Como uma boa prática de segurança, considere a utilização do comando **Executar como** para efectuar este procedimento.

Para abrir a página **Administração Global**, clique em **Iniciar**, aponte para **Todos os programas**, aponte para **Windows RMS** e clique em **Administração do Windows RMS**.

Os Domínios de Utilizadores Fidedignos permitem ao servidor do RMS fornecer licenças aos utilizadores cujos certificados de conta (RACs) foram atribuídos por outro servidor RMS.

Exportar um Domínio de Utilizadores Fidedignos
----------------------------------------------

#### Para Exportar um Domínio de Utilizadores fidedignos

1.  Na página **Políticas de fidedignidade**, na área **Domínios de publicação fidedignos**, clique em **Exportar**.

2.  Aparece a caixa de diálogo **Transferência de ficheiros**. Clique em **Guardar**.

3.  Aparece a caixa de diálogo **Guardar como**. Recomendamos que altere o nome de ficheiro .bin para incluir o nome do servidor, como RMS\_Server1\_LicensorCert.bin.

    Por predefinição, o ficheiro é guardado no ambiente de trabalho. Pode especificar uma localização diferente, se necessário.

4.  Clique em **Guardar** para guardar o ficheiro no nome da localização que especificou.

Para mais informações sobre como efectuar este procedimento, consulte "[Adicionar e Remover Domínios de Utilizadores Fidedignos](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)" anteriormente nesta secção.
