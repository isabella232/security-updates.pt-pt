---
TOCTitle: Configurar um Controlador de Domínio e o Servidor de Bases de Dados
Title: Configurar um Controlador de Domínio e o Servidor de Bases de Dados
ms:assetid: 'd20f8305-9f9e-4760-bfbf-82824db60d1f'
ms:contentKeyID: 18124171
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747681(v=WS.10)'
---

Configurar um Controlador de Domínio e o Servidor de Bases de Dados
===================================================================

Antes de instalar um servidor de certificações de raiz ou de licenciamento, certifique-se de que implementou o suporte de domínio e de base de dados adequado utilizando o Active Directory e um servidor de bases de dados, tais como o SQL Server 2000 com o Service Pack 3 (SP3) ou o Microsoft® SQL Server 2000 Desktop Engine (MSDE 2000) Release A. Embora o ambiente de produção possa já ter os componentes necessários, recomenda-se que não utilize o ambiente de produção para fins de teste.

Os procedimentos seguintes configuram um controlador de domínio e um servidor de bases de dados num computador numa rede isolada para fins de teste no lado do servidor.

| ![](/security-updates/images/Cc747681.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                                                                |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Neste exemplo, o servidor de bases de dados é executado no controlador de domínio. Num ambiente de produção, não se recomenda alojar outros componentes num controlador de domínio. Neste exemplo, o Active Directory e o servidor de bases de dados são instalados no mesmo computador para activar a instalação de uma infra-estrutura completa num número mínimo de computadores. |

Se optar por utilizar o MSDE 2000 como servidor de bases de dados, lembre-se de que não suporta interfaces de rede e que os termos de utilização do MSDE 2000 especificam que não é possível utilizar ferramentas de cliente de SQL Server para manipular uma base de dados do MSDE. Com esta restrição, não é possível ver informações de registo nem alterar dados armazenados na base de dados de configuração. Assim, recomendamos que o MSDE 2000 seja apenas utilizado para suportar as bases de dados do RMS em ambientes de teste.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Componente da Infra-estrutura</th>
<th>Passos de Configuração de um Controlador de Domínio e do Servidor de Bases de Dados</th>
<th>Notas sobre a Implementação num Ambiente de Produção</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Sistema operativo</td>
<td style="border:1px solid black;">Num ambiente que satisfaça os requisitos de hardware do RMS e que ainda não esteja ligado a uma rede, instale o Windows 2000 Server com o SP3 ou posterior ou o Windows Server 2003. Utilize o sistema de ficheiros NTFS na partição.</td>
<td style="border:1px solid black;">Recomendamos que instale sempre o service pack e as actualizações mais recentes. Utilize as partições formatadas para NTFS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ligação de rede</td>
<td style="border:1px solid black;">Estabeleça ligação com a rede que fornece conectividade de Internet mas que esteja isolada do ambiente de produção.</td>
<td style="border:1px solid black;">A ligação à Internet deve ter uma firewall adequada.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Endereço IP</td>
<td style="border:1px solid black;">Atribua um endereço IP estático a este computador.</td>
<td style="border:1px solid black;">Utilize sempre endereços IP estáticos para servidores.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Active Directory</td>
<td style="border:1px solid black;">Inicie sessão como administrador local.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Clique em <strong>Iniciar</strong>, clique em <strong>Executar</strong>, escreva <code>dcpromo</code> na caixa <strong>Abrir</strong> e, em seguida, clique em <strong>OK</strong>.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Quando o Assistente de Instalação do Active Directory se iniciar, utilize-o para criar um domínio novo numa floresta nova aceitando as opções predefinidas à excepção das seguintes:
Especifique o nome do domínio. Por exemplo, especifique contoso.com.
Deixe o assistente configurar o DNS no computador.
Seleccione <strong>Permissões compatíveis apenas com servidores Windows 2000</strong> se todos os controladores de domínio tiverem o Windows 2000 ou posterior.
Forneça uma palavra-passe segura para o administrador local.</td>
<td style="border:1px solid black;">Se necessitar de domínios novos para implementar o RMS, configure-os no Active Directory.
Utilize sempre palavras-passe seguras para todas as contas.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Reinicie o computador logo que tal lhe for pedido.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Verifique o nível funcional. Para tal, abra o snap-in <strong>Utilizadores e Computadores do Active Directory</strong>, clique com o botão direito do rato no nome do domínio, clique em <strong>Propriedades</strong> e, em seguida, verifique a definição apresentada na caixa <strong>Modo de operação do domínio</strong>. Se não existirem controladores de domínio anteriores aos do Windows 2000, clique em <strong>Alterar modo</strong> para que o domínio funcione em <strong>Modo nativo</strong>.
Nota: No Windows Server 2003, a definição <strong>Modo de operação do domínio</strong> é substituída pelo <strong>Nível de funcionalidade do domínio</strong>.</td>
<td style="border:1px solid black;">Para obter um nível óptimo de segurança e gestão, não deve utilizar o nível de funcionalidade misto do Windows 2000 para o suporte do RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Contas de utilizadores</td>
<td style="border:1px solid black;">Crie uma conta de utilizador de domínio para utilizar como conta de serviço do RMS, tal como ContosoRMS@contoso.com. Especifique uma palavra-passe segura. Não se esqueça de especificar um endereço de correio electrónico para o utilizador. Se o endereço de correio electrónico não for especificado no Active Directory, o utilizador não consegue obter licenças nem certificados a partir do RMS.
Nota: A conta de serviço do RMS não pode ser a mesma conta de domínio que foi utilizada para instalar o RMS.</td>
<td style="border:1px solid black;">Deve criar uma conta separada no Active Directory para ser utilizada pela conta de serviço do RMS. Inclua um endereço de correio electrónico. Não atribua à conta nenhumas permissões especiais.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2000</td>
<td style="border:1px solid black;">Inicie sessão no servidor em que pretende instalar a base de dados. Se esse servidor for o mesmo do controlador de domínio, terá de iniciar a sessão como administrador de domínio.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Siga as instruções fornecidas com o software de base de dados para instalar o software do servidor de bases de dados.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Utilize os procedimentos recomendados do servidor para instalar o servidor de bases de dados. Por exemplo:
<ul>
<li>Forneça um nome para a conta de administrador do sistema de bases de dados e um nome de organização, tal como Contoso.<br />
<br />
</li>
<li>Forneça uma palavra segura de administrador do sistema.<br />
<br />
</li>
<li>Utilize os métodos de autenticação integrados do Windows.<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Deve utilizar um Modo de Autenticação integrado do Windows. Se não conseguir executar o servidor de bases de dados neste modo, contacte o administrador do domínio e o administrador do servidor de bases de dados para determinar as alterações necessárias à configuração do RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Verifique se o serviço de base de dados parou.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Instale as actualizações de software no servidor de bases de dados. Se lhe for solicitada a introdução de uma palavra-passe, utilize a mesma palavra-passe especificada durante a instalação.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Reinicie o computador. Verifique se o serviço de base de dados foi iniciado.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Verifique se as contas de utilizadores têm atributos de endereço de correio electrónico válidos no Active Directory.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certifique-se de que o utilizador do domínio que irá administrar o RMS (e aprovisionar os servidores de certificações de raiz e de licenciamento) tem as permissões de servidor de bases de dados necessárias. Se estiver a utilizar o SQL Server como servidor de bases de dados, pode adicionar um identificador de início de sessão para o utilizador que está a utilizar o snap-in <strong>SQL Server Enterprise Manager</strong>. No snap-in, expanda o servidor e o grupo de servidores e, em seguida, expanda o item <strong>Security</strong>. Clique no item <strong>Logins</strong>, adicione um início de sessão novo para a conta de domínio do utilizador, clique no separador <strong>Server Roles</strong> e, em seguida, seleccione a caixa de verificação <strong>Server Administrators</strong>.</td>
<td style="border:1px solid black;">Importante: Todos os utilizadores e grupos que utilizam o RMS para adquirir licenças e publicar conteúdo devem ter um endereço de correio electrónico configurado na conta no snap-in Utilizadores e Grupos do Active Directory da MMC, no separador <strong>Geral</strong> das <strong>Propriedades</strong> do utilizador.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ligação à Internet
(opcional)</td>
<td style="border:1px solid black;">Verifique se o browser e o servidor (incluindo qualquer configuração de servidor proxy necessária), o TCP/IP e o LMHOSTS/HOSTS estão configurados correctamente para acederem à Internet. Teste indo para http://uddi.microsoft.com. Se conseguir abrir esta página, o RMS pode ligar-se ao Serviço de Inscrição da Microsoft.</td>
<td style="border:1px solid black;">Vá até http://uddi.microsoft.com para verificar o acesso à Internet.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Actualizações de software</td>
<td style="border:1px solid black;">Transfira e instale as actualizações mais recentes do software instalado neste computador (incluindo as actualizações mais recentes do Windows a partir de www.microsoft.com).</td>
<td style="border:1px solid black;">Transfira e instale sempre as actualizações mais recentes dos service packs.</td>
</tr>
</tbody>
</table>
  
Depois de executar todos os passos anteriores, pode efectuar a configuração inicial (incluindo a instalação do software de pré-requisito) nos computadores que irão executar o RMS.
