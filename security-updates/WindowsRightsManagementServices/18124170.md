---
TOCTitle: Modificar as Definições do Registo do Grupo de Ligações
Title: Modificar as Definições do Registo do Grupo de Ligações
ms:assetid: 'c61d91db-a1ad-4ca5-a492-015da629afbc'
ms:contentKeyID: 18124170
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747660(v=WS.10)'
---

Modificar as Definições do Registo do Grupo de Ligações
=======================================================

Para melhorar o desempenho do sistema, pode utilizar entradas de chaves do registo para definir as propriedades do grupo da ligação LDAP utilizado pelo RMS.

Em computadores com a versão de 32 bits do Windows Server 2003, a chave de registo seguinte é o caminho completo da subchave das entradas de registo do grupo de ligações:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Em computadores com a versão de 64 bits do Windows Server 2003, a chave de registo seguinte é o caminho completo da subchave das entradas de registo do grupo de ligações:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

A tabela seguinte mostra as entradas que pode adicionar para substituir as predefinições do grupo de ligações do Active Directory. Os valores apresentados são os predefinidos. Para mais informações sobre a forma como o RMS constrói uma lista de consultas e utiliza essas definições, consulte "Optimizar as Definições do Grupo de Ligações do Active Directory" anteriormente nesta secção.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Tipo</th>
<th>Valor Predefinido</th>
<th>Descrição</th>
<th>Notas</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GC</td>
<td style="border:1px solid black;">String</td>
<td style="border:1px solid black;">name-1, ..., name-n</td>
<td style="border:1px solid black;">Lista separada por vírgulas dos catálogos globais (utilizando nomes DNS). Esta chave obriga o RMS a utilizar apenas os catálogos globais especificados.</td>
<td style="border:1px solid black;">Se não desejar que o RMS crie uma lista de consultas, utilize esta definição para especificar quais os catálogos globais que devem ser utilizados.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MinGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Número mínimo de catálogos globais que devem estar disponíveis antes de o RMS iniciar.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MaxGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">15</td>
<td style="border:1px solid black;">Número máximo de catálogos globais que o algoritmo de identificação de topologia vai adicionar à lista de consultas.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ThreshHoldAlive</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Número mínimo de ligações que devem ter capacidade de resposta antes de os serviços de identificação começarem a procurar catálogos globais para adicionar à lista de consultas, para permitir ao RMS aceitar pedidos.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Número de vezes que se deve tentar comunicar com uma ligação que não responde até a declarar como incapaz de responder.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TimeRetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">300</td>
<td style="border:1px solid black;">Número de segundos de intervalo entre as várias tentativas para comunicar com uma ligação que não responde.</td>
<td style="border:1px solid black;">Não deve ser necessário alterar este valor predefinido, excepto em circunstâncias muito especiais.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeRetrySlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">30</td>
<td style="border:1px solid black;">Número de segundos de intervalo entre as várias tentativas para comunicar com uma ligação lenta.</td>
<td style="border:1px solid black;">Não deve ser necessário alterar este valor predefinido, excepto em circunstâncias muito especiais.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtRoundRobin</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Peso do “round robin” durante o balanceamento de carga.</td>
<td style="border:1px solid black;">A importância relativa do “round robin” no balanceamento de carga. O valor 1 é o mais baixo.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WtThreadCount</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">100</td>
<td style="border:1px solid black;">Peso do número de threads por ligação durante o balanceamento de carga.</td>
<td style="border:1px solid black;">A importância relativa de um baixo número de threads.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtSlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Peso da ligação lenta durante o balanceamento de carga.</td>
<td style="border:1px solid black;">A importância relativa da ligação não ser lenta.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeOutForGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Número de segundos a esperar até dar como excedido o tempo para responder a um pedido de adicionar um catálogo global à lista de consultas.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">LdapTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Número de segundos a esperar até que as APIs do LDAP sejam desligadas.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TopDownExpansionLDAPTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">40</td>
<td style="border:1px solid black;">Número de segundos a esperar até que as consultas de expansão, da primeira à última, do LDAP sejam desligadas.</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc747660.Caution(WS.10).gif)Atenção                                                                                                                  |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Uma edição incorrecta do registo pode danificar gravemente o sistema. Antes de proceder a alterações do registo, faça uma cópia de segurança dos dados importantes que guarda no computador. |
