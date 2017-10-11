---
TOCTitle: 'Passo 4: Sincronizar o Servidor'
Title: 'Passo 4: Sincronizar o Servidor'
ms:assetid: 'a5514e46-a50b-46a6-9e5b-33c87c5b7cef'
ms:contentKeyID: 18142257
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc708523(v=WS.10)'
---

Passo 4: Sincronizar o Servidor
===============================

Depois de configurar a ligação de rede, poderá obter actualizações. Por predefinição, o WSUS está configurado para transferir Actualizações Críticas e de Segurança para todos os produtos Microsoft. Para obter actualizações, terá de *sincronizar* o servidor WSUS.

A sincronização implica que o servidor WSUS contacte o Microsoft Update. Após o contacto, o WSUS determina se foram disponibilizadas novas actualizações desde a última sincronização. Dado que se trata da primeira vez que está a sincronizar o servidor WSUS, todas as actualizações estão disponíveis e prontas para aprovação para instalação.

| ![](images/Cc708523.note(WS.10).gif)Nota                                                                                                                                                                                                                       |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Esta documentação descreve como sincronizar utilizando-se predefinições, mas o WSUS inclui opções que lhe permitem minimizar a utilização de largura de banda durante a sincronização. Para mais informações, consulte a documentação “Deploying Microsoft Server Windows Update Services”. |

**Para sincronizar o servidor WSUS**
1.  Na barra de ferramentas da consola WSUS, clique em **Opções** e, em seguida, clique em **Opções de Sincronização**.

2.  Em **Tarefas**, clique em **Sincronizar agora**.

Quando a sincronização estiver concluída, clique em **Actualizações** na barra de ferramentas da consola WSUS para ver a lista de actualizações.
