---
TOCTitle: 'Alterar a Palavra-passe da Conta de Serviço do RMS'
Title: 'Alterar a Palavra-passe da Conta de Serviço do RMS'
ms:assetid: '435c9cef-b622-48b3-9d4d-4bf5cac7d52d'
ms:contentKeyID: 18123959
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720273(v=WS.10)'
---

Alterar a Palavra-passe da Conta de Serviço do RMS
==================================================

Dependendo da política de palavra-passe especificada para os servidores do RMS, a palavra-passe da conta de serviço do RMS pode expirar periodicamente. Se a palavra-passe expirar, o RMS pára de funcionar. Por esta razão, deve alterar a palavra-passe antes da sua expiração.

**Utilizar uma Conta de Serviço do RMS**

Quando se utiliza uma conta de serviço do RMS, pode-se alterar a palavra-passe de cada servidor do RMS da seguinte maneira:

1.  Se o servidor estiver num cluster, retire-o de rotação.
2.  Inicie a sessão no servidor utilizando as credenciais da conta de serviço do RMS.
3.  Altere a palavra-passe da conta de serviço do RMS.
    Outros servidores com a mesma conta de serviço do RMS ficarão fora de serviço porque as credenciais neles armazenadas ficarão inválidas após a alteração da palavra-passe.
4.  Termine a sessão no servidor.
5.  Inicie a sessão no servidor, utilizando as credenciais de administrador do RMS.
6.  Para reconfigurar a ID de utilizador no servidor, na página **Administração Global**, clique em **Alterar a conta de serviço do RMS**, e, na página **Alterar a conta de serviço do RMS**, especifique o domínio, nome de utilizador e palavra-passe.
7.  Reinicie o IIS.
8.  Caso se aplique, volte a colocar o servidor em rotação.
9.  Repita os passos 6 a 8 para cada um dos servidores do cluster.

Esta é a abordagem mais simples para alterar a palavra-passe da conta de serviço do RMS; no entanto, poderá resultar num certo tempo de paragem do RMS porque o Active Directory é actualizado com a nova palavra-passe quando altera a palavra-passe da conta de serviço do RMS num servidor. Os Serviços de Informação Internet reiniciam os grupos de aplicações e os grupos de aplicações que estão a ser executados com credenciais antigas não podem ser iniciados enquanto a palavra-passe da conta de serviço do RMS não for alterada e os IIS forem reiniciados nesse servidor. O RMS não funciona enquanto os grupos de aplicações não voltarem a ser executados.

**Utilizar Duas Contas de Serviço do RMS**

Com este método, crie primeiro duas contas de serviço do RMS com políticas ou datas de expiração diferentes. Sob condições normais de funcionamento, o RMS opera sob a primeira conta. Quando estiver pronto para alterar a palavra-passe da primeira conta, execute os seguintes passos em cada servidor do RMS:

1.  Se o servidor estiver num cluster, retire-o de rotação.
2.  Especifique a segunda conta de serviço do RMS como sendo a conta sob a qual opera o RMS. Para mais instruções para a alteração da conta, consulte "[Alterar a Conta de Serviço do RMS](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)" posteriormente nesta secção.
3.  Reinicie o IIS.
4.  Caso se aplique, volte a colocar o servidor em rotação.

Assim que todos os servidores do RMS estiverem a utilizar a segunda conta de serviço do RMS, pode alterar a palavra-passe da primeira conta de serviço do RMS sem afectar o funcionamento do sistema do RMS. Pode também alternar desta forma entre as duas contas, evitando assim a paragem do RMS.
