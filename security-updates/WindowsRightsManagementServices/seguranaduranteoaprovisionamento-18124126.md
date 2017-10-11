---
TOCTitle: Segurança Durante o Aprovisionamento
Title: Segurança Durante o Aprovisionamento
ms:assetid: '9f1282c5-5642-4870-a9a4-c3a485f8ff76'
ms:contentKeyID: 18124126
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747616(v=WS.10)'
---

Segurança Durante o Aprovisionamento
====================================

Pode utilizar o Web site Administração do RMS para aprovisionar recursos do RMS num Web site existente. Durante o aprovisionamento, os directórios virtuais e os grupos de aplicações são criados neste Web site e as bases de dados do RMS são criadas e configuradas num servidor de bases de dados. Opcionalmente, se o servidor estiver ligado à Internet, pode ser inscrito através do Serviço de Inscrição da Microsoft durante o processo de aprovisionamento.

Durante o aprovisionamento, o RMS utiliza as contas descritas na tabela a seguir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Conta</th>
<th>Finalidade</th>
<th>Permissões</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Conta do utilizador em sessão</td>
<td style="border:1px solid black;">Cria directórios virtuais e grupos de aplicações. O IIS requer a autenticação do Windows e o RMS representa o utilizador com sessão iniciada que tem de iniciar sessão localmente.</td>
<td style="border:1px solid black;">Controlo total (o utilizador em sessão tem de ser um administrador local).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Conta de sistema</td>
<td style="border:1px solid black;">Constrói a assemblagem temporária para a serialização.</td>
<td style="border:1px solid black;">Permissões de Leitura e de Escrita para a pasta temporária do Windows, C:\Windows\Temp.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Conta ASPNET</td>
<td style="border:1px solid black;">Cria a assemblagem temporária dos ficheiros *.aspx.</td>
<td style="border:1px solid black;">Acesso ao directório da cache de assemblagem temporária, por predefinição o C:\Windows\Microsoft.NET\Framework\v1.1.4322\Temporary ASP.NET Files.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Conta de Serviços de rede</td>
<td style="border:1px solid black;">Regista o ponto de ligação do serviço no Active Directory.</td>
<td style="border:1px solid black;"><ul>
<li>Permissões Só de Leitura para o site de aprovisionamento (geralmente o C:\Inetpub\Wwwroot\Provisioning).<br />
<br />
</li>
<li>Permissões de Leitura e Escrita para a chave de registo <strong>DRMS</strong>. As permissões são concedidas pelo programa de configuração do RMS que também cria a chave de registo seguinte.<br />
<br />
Em computadores com a versão de 32 bits do Windows Server 2003:<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0</code><br />
<br />
Em computadores com a versão de 64 bits do Windows Server 2003:<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0</code><br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

Durante o aprovisionamento, o RMS executa as seguintes tarefas:

-   No servidor de bases de dados:
    -   Cria as bases de dados de configuração, de serviços de directório e de registo.
    -   Concede permissões de Início de Sessão ao RMS Service Group.
    -   Instala procedimentos armazenados nas bases de dados e concede permissões de Execução ao RMS Service Group.
    -   Executa consultas à base de dados principal.
-   Adiciona o RMS Service Group ao grupo IIS\_WPG.
-   Em C:\\Inetpub\\Wwwroot\\\_wmcs, cria uma hierarquia de directórios virtuais, ficheiros e grupos de aplicações para os serviços Web e para o Web site Administração do RMS.
-   Define DACLs nos directórios virtuais, ficheiros e grupos de aplicações.
-   Ao RMS Service Group, concede acesso à pasta temporária.
-   Quando se especifica a protecção de chaves por meio de software, encripta a chave privada do servidor de licenciadores antes de a armazenar na base de dados. O RMS pede uma palavra-passe durante o aprovisionamento e obtém acesso ao DPAPI a nível de máquina.
-   Instala o serviço de escuta do registo.
-   Cria uma fila de mensagens de registo.
-   Se estiver a aprovisionar o servidor de certificações de raiz, define o ponto de ligação do serviço no Active Directory.
