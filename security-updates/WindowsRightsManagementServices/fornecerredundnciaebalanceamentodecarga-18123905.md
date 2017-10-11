---
TOCTitle: Fornecer Redundância e Balanceamento de Carga
Title: Fornecer Redundância e Balanceamento de Carga
ms:assetid: '162d547c-78a7-4848-b43e-58e481832af2'
ms:contentKeyID: 18123905
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720199(v=WS.10)'
---

Fornecer Redundância e Balanceamento de Carga
=============================================

Para garantir que os utilizadores podem adquirir licenças e publicar conteúdo sempre que for necessário, recomendamos que implemente servidores redundantes do RMS através da utilização de clusters. No mínimo, isto implica a implementação de um cluster de certificações de raiz com, pelo menos, dois servidores. Se implementar também um servidor de licenciamento separado para suportar necessidades de licenciamento específicas de um grupo individual da organização, deve implementar o servidor de licenciamento como um cluster com, pelo menos, dois servidores.

Os múltiplos servidores físicos do cluster de certificações de raiz ou de qualquer cluster de licenciamento constituem uma "Web farm" baseada num URL partilhado ou num endereço virtual. Se a organização utilizar uma farm de servidores, pode integrar o RMS na técnica aplicada ao endereçamento virtual, tal como o DNS de round-robin, o serviço Balanceamento de Carga em Rede ou uma solução de hardware dedicada.

Para além do balanceamento de carga, o endereçamento virtual pode ser vantajoso quando o utiliza com o RMS pois remove a dependência de qualquer servidor físico para os serviços de certificação ou licenciamento. Nenhum computador de utilizador final requer acesso directo a um só servidor que esteja num cluster.
