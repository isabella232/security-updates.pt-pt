---
TOCTitle: Trabalhar com Modelos de Política de Direitos
Title: Trabalhar com Modelos de Política de Direitos
ms:assetid: 'ff4f1143-f6b9-4dd8-aa4c-c2cbbf6fdf06'
ms:contentKeyID: 18124240
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747804(v=WS.10)'
---

Trabalhar com Modelos de Política de Direitos
=============================================

Depois de criar um modelo de política de direitos, é possível gerir a forma como ele é aplicado na organização controlando a forma como ele é distribuído aos autores.

O RMS guarda os modelos de política de direitos na base de dados de configuração. Além disso, mantém uma cópia de todos os modelos de política de direitos numa pasta partilhada que tenha sido especificada, como descrito em "[Para Especificar a Localização dos Modelos de Política de Direitos](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)" nesta secção. Deve certificar-se de que os modelos ficam guardados numa localização acessível da rede que satisfaça as linhas gerais de segurança da sua empresa. Não devem ser criadas pastas partilhadas para modelos nas pastas principais utilizadas pelo RMS, tais como a pasta Programas ou as pastas IISRoot.

Quando publica conteúdos protegidos, o autor selecciona o modelo de política de direitos a aplicar nos modelos que se encontram disponíveis no computador local. Para que os modelos de política de direitos fiquem disponíveis para utilização, o administrador tem de os implementar nos computadores dos utilizadores de uma pasta partilhada.

Quando um utilizador tenta consumir conteúdo protegido, a aplicação activada pelo RMS obtém a última versão do modelo de política de direitos que foi utilizado para publicar o conteúdo da base de dados de configuração. A aplicação activada pelo RMS aplica então estas definições ao conteúdo. Quando modificar um modelo da política de direitos no servidor do RMS, o RMS actualiza o modelo em conformidade na base de dados de configuração e na pasta partilhada (se o servidor do RMS for configurado para especificar a localização de um ficheiro para armazenar cópias dos modelos da política de direitos). Implemente novamente o modelo de política de direitos nos sistemas do cliente quando é modificado, para que os utilizadores fiquem com a versão mais actual disponível nos computadores.

Se eliminar um modelo de política de direitos, este é removido da base de dados de configuração e da localização da pasta partilhada (que é especificada como a localização de ficheiros para o armazenamento de cópias de modelos) quando elimina o modelo. Contudo, não é removido dos computadores dos utilizadores. Terá de o remover dos computadores manualmente. Os modelos de política de direitos eliminados devem ser removidos de todos os computadores dos utilizadores. Se não o fizer e o modelo de política de direitos eliminado for utilizado para publicar conteúdos, o RMS não conseguirá emitir nenhuma licença de utilização para o conteúdo, porque não consegue localizar o modelo especificado na base de dados de configuração.

Ao trabalhar com modelos de política de direitos devem efectuar-se as seguintes tarefas:

-   **Especificar uma pasta partilhada**. Antes de ser criado o primeiro modelo de política de direitos, tem de se especificar a pasta partilhada onde todos os modelos de política de direitos vão ser guardados. Para mais informações, consulte "[Para Especificar a Localização dos Modelos de Política de Direitos](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)" posteriormente nesta secção.
-   **Criar e editar modelos de política de direitos**. É possível criar tantos modelos de política de direitos quantos forem necessários para gerir os direitos dentro de uma organização. Quando um modelo de política de direitos é criado, são definidos os utilizadores e os direitos aplicáveis. É também definida a forma como o modelo de política de direitos deve ser aplicado ao conteúdo. Mais tarde, os modelos de política de direitos podem ser editados, se necessário, para actualização. Para mais informações, consulte "[Criar e Modificar Modelos de Política de Direitos](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" posteriormente nesta secção.
-   **Distribuir modelos de política de direitos**. Para um autor aplicar um determinado modelo de política de direitos a um conteúdo, tem de existir uma cópia desse modelo no computador do autor. É possível controlar que autores aplicam que modelos de política de direitos através de uma gestão da distribuição dos modelos. Para mais informações, consulte "[Distribuir Modelos de Política de Direitos](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe)" posteriormente nesta secção.
-   **Retirar modelos de políticas de direitos**. Quando um modelo de política de direitos deixa de ser apropriado, pode ser eliminado. Quando o fizer, tem também de o remover dos computadores dos utilizadores, para que estes não venham a ter problemas quando tentarem consumir conteúdos que foram publicados utilizando o modelo de política de direitos que foi retirado. Para mais informações, consulte "[Retirar Modelos de Política de Direitos](https://technet.microsoft.com/32bf98c7-edda-4507-a4b8-4c11bddd6e60)" posteriormente nesta secção.
