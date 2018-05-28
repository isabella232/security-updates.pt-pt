---
TOCTitle: Desinstalar e Desaprovisionar o RMS
Title: Desinstalar e Desaprovisionar o RMS
ms:assetid: 'cae1ed5b-f716-41f0-8e14-7cbfef405331'
ms:contentKeyID: 18124158
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747753(v=WS.10)'
---

Desinstalar e Desaprovisionar o RMS
===================================

Poderá ser necessário, por várias razões, remover o RMS de um servidor. No caso de um servidor de certificações de raiz, o primeiro passo é desaprovisionar o RMS no servidor. Pode fazê-lo a partir da página **Administração Global** do servidor que pretende desaprovisionar, clicando em **Remover o RMS deste Web site**. Não necessita de desaprovisionar um servidor de licenciamentos antes de desinstalar o RMS.

| ![](/security-updates/images/Cc747753.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                                                                                     |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Quando se desaprovisiona o último servidor de certificações de raiz que se encontra numa floresta do Active Directory, o objecto do ponto de ligação do serviço é removido do Active Directory. Se não desaprovisionar esse servidor antes de desinstalar o RMS, não é possível aprovisionar um novo servidor de certificações de raiz nessa floresta enquanto o objecto do ponto de ligação do serviço não for removido manualmente do Active Directory. |

De seguida, desinstale o RMS.

Quando se desaprovisiona e desinstala o RMS de um servidor autónomo ou do último servidor de um cluster, é removida a base de dados de serviços de directório. As bases de dados de configuração e registo não são removidas; no entanto, se actualizar ou reinstalar o RMS no servidor, a base de dados de registo será substituída por uma nova.

Quando se desaprovisiona e desinstala o RMS de um servidor que faz parte de um cluster, as bases de dados de configuração, registo e serviços de directório para o cluster não são removidas. No entanto, a tabela DRMS\_ClusterServer da base de dados de configuração é actualizada de forma a indicar que o servidor foi removido do cluster.

Para mais informações sobre como retirar servidores e as suas implicações, consulte "[Retirar Servidores](https://technet.microsoft.com/52005e2e-9563-4ba0-906c-3cc76f9c378f)" anteriormente nesta secção.
