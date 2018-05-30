---
TOCTitle: Definir os Requisitos de Gestão de Chaves
Title: Definir os Requisitos de Gestão de Chaves
ms:assetid: 'f0e08fb8-bf5e-4278-a09f-daa57696e786'
ms:contentKeyID: 18124248
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747797(v=WS.10)'
---

Definir os Requisitos de Gestão de Chaves
=========================================

O RMS utiliza chaves criptográficas para fornecer protecção de conteúdo e impor direitos. As chaves criptográficas são peças fundamentais de informação que permitem ao sistema trabalhar de forma segura e sem interrupções. Os administradores devem ter especial cuidado a gerir essas chaves a fim de as proteger contra a perda de dados, falhas de sistema e roubo.

Na configuração predefinida, o RMS armazena o par de chaves de servidor e os GUID associados numa tabela na base de dados de configuração. O par de chaves de servidor é encriptado pela palavra-passe seleccionada durante o processo de aprovisionamento.

Para proteger o par de chaves do servidor e o GUID associado, efectue uma cópia de segurança da base de dados de configuração para o suporte de dados de armazenamento (por exemplo, um CD) e, em seguida, coloque o suporte de cópia de segurança num local seguro (por exemplo, um cofre fora das instalações). O agendamento das cópias de segurança depende da frequência das alterações administrativas e do nível de risco aceitável de perda de dados devido à degradação do suporte de dados ou de outros riscos associados a suportes de dados. Certifique-se de que existe uma forma de identificar a palavra-passe da chave privada que está a ser utilizada para a base de dados de configuração de cópia de segurança. Sem a palavra-passe adequada, não será capaz de restaurar a cópia de segurança para o servidor do RMS.

Se estiver a utilizar o SQL Server como servidor de bases de dados, pode utilizar o SQL Server Enterprise Manager para copiar directamente o valor dos dados de chave privada encriptada e do GUID para uma disquete segura ou outro suporte de dados. Como a chave privada se encontra protegida, a instalação do RMS tem de ser executada na mesma conta de serviço do RMS utilizada pela cópia de segurança, caso a restaure a partir do suporte de dados seguro para uma instalação do RMS.

Se utilizar um CSP de software ou de hardware para proteger a chave privada do servidor, tem de criar manualmente uma cópia de segurança do contentor de chaves e da chave. Quando utiliza um módulo de segurança por hardware, a segurança das chaves privadas é melhorada dado que as chaves privadas são mantidas no hardware e nunca são expostas ao software. Os dados que necessitam de ser desencriptados ou assinados são enviados para o módulo de segurança do hardware, desencriptados ou assinados e, em seguida, enviados para fora.

Cada CSP, quer seja de hardware ou de software, tem procedimentos específicos para a execução de cópias de segurança de chave com segurança. Se não estiver familiarizado com este procedimento, consulte a documentação do CSP.
