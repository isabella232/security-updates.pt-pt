---
TOCTitle: Manter a Base de Dados dos Serviços de Directório
Title: Manter a Base de Dados dos Serviços de Directório
ms:assetid: '911a62f2-c1d6-4091-99b0-b53211be27a7'
ms:contentKeyID: 18124099
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747680(v=WS.10)'
---

Manter a Base de Dados dos Serviços de Directório
=================================================

O RMS inclui uma base de dados de serviços de directório alojada no servidor de bases de dados que contém informações sobre os utilizadores, identificadores (tais como endereços de correio electrónico), IDs de segurança (SIDs), membros de grupo e identificadores alternativos. Estas informações são obtidas através de consultas LDAP efectuadas no catálogo global do Active Directory pelo serviço de licenciamento do RMS e colocadas na cache local desta base dados para melhorar o tempo de resposta do servidor quando os utilizadores pedem licenças de utilização.

Como os dados armazenados nesta base de dados são inseridos e eliminados frequentemente, existe uma tendência para a fragmentação. Periodicamente (diária ou semanalmente), efectue uma reorganização de base de dados para os índices de todas as tabelas de bases de dados DRMS\_DirectoryServices. Isto recria os índices para que os dados deixem de estar fragmentados. Os dados fragmentados podem diminuir o desempenho e até resultar em falha do servidor se não existir uma intervenção administrativa.

Se estiver a utilizar o SQL Server como servidor de bases de dados, as reorganizações de bases de dados podem ser efectuadas com o Maintenance Wizard ou executando um script personalizado através do SQL Server Agent.

Se detectar que o registo de transacção tem um tamanho inaceitável quando reindexar a base de dados, reduza o tamanho comutando do modo de recuperação total para o modo de registo de massa antes da reindexação.
