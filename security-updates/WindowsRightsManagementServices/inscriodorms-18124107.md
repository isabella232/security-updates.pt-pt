---
TOCTitle: Inscrição do RMS
Title: Inscrição do RMS
ms:assetid: '999db3e1-e3ab-4513-87d9-d584ee334c00'
ms:contentKeyID: 18124107
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747698(v=WS.10)'
---

Inscrição do RMS
================

O processo de inscrição do servidor cria e entrega um certificado de licenciador de servidores. Os certificados de licenciador de servidores validam a identidade dos servidores existentes na implementação, fornecendo validação de credenciais durante o consumo de conteúdo protegido pelo RMS. O primeiro servidor de cada cluster de licenciamento é inscrito com o cluster de certificações de raiz como parte do processo de aprovisionamento. Os servidores subsequentes existentes no cluster não são inscritos separadamente.

O servidor inicial de um cluster de certificações de raiz (o servidor de certificação de raiz) deve ser inscrito no Serviço de Inscrição da Microsoft. Este processo pode ser efectuado automaticamente como parte do aprovisionamento quando o servidor de certificação de raiz está ligado à Internet. Alternativamente, o processo de inscrição pode ser concluído offline através da exportação de um pedido para um ficheiro e, em seguida, submetendo o ficheiro ao Serviço de Inscrição da Microsoft a partir de outro computador com ligação à Internet. O pedido de inscrição devolve um certificado de licenciador de servidores para o servidor de certificação de raiz que pode ser importado através das páginas Web Administração do RMS.

O pedido de inscrição inclui as seguintes informações:

-   Informações de revogação. Se a instalação do RMS utiliza a revogação padrão ou personalizada (de terceiros). Se estiver a ser utilizada a revogação de terceiros, a chave pública da autoridade de revogação é incluída.
-   Chave Pública do Certificado. A chave pública do certificado de licenciador de servidores. Esta chave pública é gerada no servidor do RMS e é enviada para o Serviço de Inscrição da Microsoft para obter o certificado de licenciador de servidores.
-   SKU. O título SKU oficial do RMS.
-   Versão. O número da versão de assemblagem do RMS.
-   URL. O URL base do cluster de servidores do RMS.

Quando o Serviço de Inscrição da Microsoft fornece uma resposta ao pedido de inscrição, as informações indicadas a seguir são devolvidas ao servidor do RMS em formato XML:

-   Certificado de Licenciador de Servidores.
-   Cadeia de certificados das entidades assinantes.

Independentemente de a inscrição do servidor de certificação de raiz do RMS ser efectuada online ou offline, são sempre transferidas as mesmas informações. Nenhum dos métodos recolhe informações adicionais.

Para obter os passos do procedimento de inscrição offline do servidor, consulte "Para Utilizar a Inscrição Offline para Inscrever um Servidor de Certificação de Raiz" em “Utilizar um Servidor do RMS” nesta colecção de documentação.

O processo de inscrição do cliente cria e entrega um certificado de licenciador de clientes que permite a um autor publicar conteúdo protegido pelo RMS a partir de um computador sem ligação à rede empresarial. Um autor pode pedir um certificado de licenciador de clientes em qualquer altura. A inscrição do cliente não é necessária.

Todos os pedidos de inscrição são registados.

Esta secção trata de:

-   [Inscrição do Servidor de Certificação de Raiz](https://technet.microsoft.com/f08bc919-f090-4843-b2ce-b40d558012ce)
-   [Pré-inscrição do Servidor de Licenciamento](https://technet.microsoft.com/7bc63397-9186-464c-8824-867038adce9b)
-   [Inscrição do Cliente do RMS](https://technet.microsoft.com/9c1d07bf-7235-4694-8291-ac2e5b221f4a)
-   [Activação de Computador do RMS](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)
-   [Certificação de Contas do RMS](https://technet.microsoft.com/c9a385c5-6dbb-47f5-a80f-69718e6f9deb)
