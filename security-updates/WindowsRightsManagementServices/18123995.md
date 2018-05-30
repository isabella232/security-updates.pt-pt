---
TOCTitle: Publicação dos Serviços do RMS
Title: Publicação dos Serviços do RMS
ms:assetid: '3cca9325-6bd3-49ad-aa3f-e0693205d3f4'
ms:contentKeyID: 18123995
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720247(v=WS.10)'
---

Publicação dos Serviços do RMS
==============================

Os URL dos serviços do RMS são publicados no Active Directory durante o aprovisionamento do servidor. Durante o aprovisionamento, o programa de configuração do RMS consulta o Active Directory para determinar se existem ou não outros servidores do RMS instalados nessa floresta. Se não existirem outros servidores do RMS instalados, o programa de configuração do RMS configura o servidor como servidor de certificações de raiz. Antes de utilizar o RMS, tem de registar o ponto de ligação de serviço (SCP) no Active Directory para que os clientes detectem o URL do servidor de certificações de raiz. Os clientes que pedirem ligações aos serviços que estão a ser executados no servidor de certificações de raiz começam por consultar o Active Directory para saber o URL desse servidor de certificações de raiz. Para mais informações, consulte "Registar o Ponto de Ligação do Serviço" em "Utilizar um Servidor do RMS" nesta colecção de documentação.

| ![](/security-updates/images/Cc720247.note(WS.10).gif)Nota                                                                                                                                                                           |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se a sua topologia incluir vários servidores que estejam num cluster de servidor de certificações de raiz, o URL aponta para o servidor de balanceamento de carga do cluster, o qual é fornecido pelo administrador durante o aprovisionamento. |
