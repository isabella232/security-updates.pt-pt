---
TOCTitle: 'MS10-OCT'
Title: Resumo dos Boletins de Segurança Microsoft de Outubro de 2010
ms:assetid: 'ms10-oct'
ms:contentKeyID: 61235163
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms10-oct(v=Security.10)'
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Outubro de 2010
=============================================================

Data de publicação: 12 de outubro de 2010 | Updated: 26 de outubro de 2011

**actualizada:** 4.1

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Outubro de 2010.

Com a publicação dos boletins de Outubro de 2010, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 7 de Outubro de 2010. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 13 de Outubro de 2010, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o Webcast de boletins de segurança de Outubro](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032454437&culture=en-us). Depois desta data, o webcast estará disponível mediante pedido. Para obter mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

A Microsoft também fornece informações para ajudar os clientes a dar prioridade às actualizações de segurança mensais com quaisquer actualizações de elevada prioridade não relacionadas com segurança que sejam lançadas no mesmo dia que as actualizações de segurança mensais. Consulte a secção: **Outras informações**.

### Informação do Boletim

Resumos Executivos
------------------

<span></span>
A tabela seguinte resume os boletins de segurança para este mês, por ordem de gravidade.

Para obter mais informações sobre o software afectado, consulte a secção seguinte, **Localizações do Software Afectado e das Transferências**.

 
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
<th style="border:1px solid black;" >Identificação do Boletim</th>
<th style="border:1px solid black;" >Título do Boletim e Resumo Executivo</th>
<th style="border:1px solid black;" >Classificação de Gravidade Máxima e Impacto da Vulnerabilidade</th>
<th style="border:1px solid black;" >Requisito de Reínicio</th>
<th style="border:1px solid black;" >Software Afectado</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=202013">MS10-071</a></td>
<td style="border:1px solid black;"><strong>Actualização de Segurança Cumulativa para o Internet Explorer (2360131)</strong><br />
<br />
Esta actualização de segurança resolve sete vulnerabilidades comunicadas de forma privada e três vulnerabilidades divulgadas publicamente no Internet Explorer. As vulnerabilidades mais graves poderiam permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201722">MS10-075</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Serviço de Partilha de Rede do Media Player Poderia Permitir Execução Remota de Código (2281679)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade, comunicada de forma privada, no serviço de partilha de rede do Microsoft Windows Media Player. A vulnerabilidade poderia permitir a execução remota de código se um intruso enviasse um pacote RTSP especialmente concebido para o efeito para um sistema afectado. No entanto, o acesso ao multimédia doméstico através da Internet está desactivado por predefinição. Nesta configuração predefinida, a vulnerabilidade apenas pode ser explorada por um intruso dentro da mesma sub-rede.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194560">MS10-076</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Motor de Tipos de Letra OpenType Incorporados Poderia Permitir Execução Remota de Código (982132)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada num componente do Microsoft Windows, o Motor de Tipos de Letra OpenType Incorporados (EOT). A vulnerabilidade poderia permitir a execução remota de código. Um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter o controlo total de um sistema afectado remotamente. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201704">MS10-077</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade</strong> <strong>no .NET Framework Poderia Permitir Execução Remota de Código (2160841)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft .NET Framework comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código num sistema cliente se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando um browser da Web que pudesse executar Aplicações de Browser XAML (XBAPs). Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. A vulnerabilidade também poderia permitir a execução remota de código num sistema de servidor a executar o IIS, se esse servidor permitisse o processamento de páginas ASP.NET e se um intruso tivesse sucesso em actualizar uma página ASP.NET especialmente concebida para o efeito para esse servidor e executá-la, como poderia ser o caso de um cenário de alojamento Web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=202016">MS10-072</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no SafeHTML Poderiam Permitir Divulgação de Informações</strong> <strong>(2412048)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente e uma vulnerabilidade comunicada de forma privada no Microsoft SharePoint e no Windows SharePoint Services. As vulnerabilidades poderiam permitir a divulgação de informações se um intruso enviasse um script especialmente concebido para o efeito para um site visado utilizando o SafeHTML.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Divulgação de Informações</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Software Microsoft Server</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201093">MS10-073</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades nos</strong> <strong>Controladores de Modo de Kernel do Windows Poderiam Permitir Elevação de Privilégios (981957)</strong><br />
<br />
Esta actualização de segurança resolve várias vulnerabilidades divulgadas de forma pública nos controladores de modo de kernel do Windows. A vulnerabilidade mais grave poderia permitir elevação de privilégios se um intruso iniciasse sessão num sistema afectado e executasse uma aplicação especialmente concebida para o efeito.
Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar esta vulnerabilidade. A vulnerabilidade não poderia ser explorada remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201084">MS10-078</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Controlador de Formato do Tipo de Letra OpenType (OTF) Poderiam Permitir Elevação de Privilégios (2279986)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades comunicadas de forma privada no controlador de formato do Tipo de Letra OpenType (OTF) do Windows. Esta actualização de segurança está classificada como Importante para todas as edições do Windows XP e Windows Server 2003 suportadas. Todas as edições suportadas do Windows Vista, Windows Server 2008, Windows 7 e Windows Server 2008 R2 não são afectadas pela vulnerabilidade.<br />
<br />
As vulnerabilidades poderiam permitir elevação de privilégios se um utilizador visualizasse conteúdo processado num tipo de letra OpenType especialmente concebido para o efeito. Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar esta vulnerabilidade. A vulnerabilidade não poderia ser explorada remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201696">MS10-079</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft Word Poderiam Permitir Execução Remota de Código (2293194)</strong><br />
<br />
Esta actualização de segurança resolve onze vulnerabilidades no Microsoft Office, comunicadas de forma privada. As vulnerabilidades poderiam permitir a execução remota de código se um utilizador abrisse um ficheiro Word especialmente concebido para o efeito. Um intruso que conseguisse explorar qualquer uma destas vulnerabilidades com sucesso poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200529">MS10-080</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft Excel Poderiam Permitir Execução Remota de Código (2293211)</strong><br />
<br />
Esta actualização de segurança resolve treze vulnerabilidades no Microsoft Office, comunicadas de forma privada. As vulnerabilidades poderiam permitir a execução remota de código se um utilizador abrisse um ficheiro Excel especialmente concebido para o efeito ou um ficheiro Lotus 1-2-3 especialmente concebido para o efeito. Um intruso que conseguisse explorar qualquer uma destas vulnerabilidades com sucesso poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201086">MS10-081</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na Biblioteca de Controlo Comum do Windows Poderia Permitir Execução Remota de Código (2296011)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade na biblioteca de controlo comum do Windows, comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um utilizador visitasse uma página Web especialmente concebida para o efeito. Se um utilizador tiver sessão iniciada com privilégios administrativos, um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter controlo total sobre um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201098">MS10-082</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade</strong> <strong>no Windows Media Player Poderia Permitir Execução Remota de Código (2378111)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Windows Media Player, comunicada de forma privada. A vulnerabilidade poderia permitir execução remota de código se fosse aberto no Windows Media Player conteúdo multimédia especialmente concebido para o efeito alojado num Web site malicioso. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190553">MS10-083</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na Validação COM na Shell do Windows e no WordPad Poderia Permitir Execução Remota de Código (2405882)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um utilizador abrisse um ficheiro especialmente concebido para o efeito com o WordPad ou se seleccionasse ou abrisse um ficheiro de atalho numa partilha de rede ou WebDAV. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201720">MS10-084</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na Chamada de Procedimento Local do Windows Poderia Permitir Elevação de Privilégios (2360937)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, divulgada publicamente. Esta actualização de segurança está classificada como Importante para todas as edições do Windows XP e Windows Server 2003 suportadas. Todas as edições suportadas do Windows Vista, Windows Server 2008, Windows 7 e Windows Server 2008 R2 não são afectadas pela vulnerabilidade.<br />
<br />
A vulnerabilidade poderia permitir elevação de privilégios se um intruso iniciasse sessão num sistema afectado e executasse código especialmente concebido para o efeito que enviasse uma mensagem LPC para o Servidor LRPC local. A mensagem poderia então permitir que um utilizador autenticado acedesse a recursos com execução no contexto da conta NetworkService. Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar esta vulnerabilidade.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201705">MS10-085</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no SChannel Poderia Permitir Negação de Serviço (2207566)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no pacote de segurança Secure Channel (SChannel) no Windows, comunicada de forma privada. A vulnerabilidade poderia permitir negação de serviço se um sistema afectado recebesse uma mensagem de pacote especialmente concebida para o efeito através do Secure Sockets Layer (SSL). Por predefinição, todas as edições suportadas do Windows Vista, Windows Server 2008, Windows 7 e Windows Server 2008 R2 não estão configuradas para receber tráfego de rede SSL.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Negação de Serviço</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201703">MS10-074</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft Foundation Classes Poderia Permitir a Execução Remota de Código (2387149)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade na Biblioteca MFC (Microsoft Foundation Class) divulgada publicamente. A vulnerabilidade poderia permitir a execução remota de código se um utilizador tivesse sessão iniciada com privilégios administrativos e abrisse uma aplicação construída com a Biblioteca MFC. Um intruso que conseguisse explorar esta vulnerabilidade com êxito poderia obter as mesmas permissões que o utilizador com sessão iniciada. Se um utilizador tiver sessão iniciada com direitos de utilizador administrativos, um intruso poderia obter controlo total sobre o sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Moderada</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201721">MS10-086</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade nos Discos de Cluster Partilhados no Windows Poderia Permitir Adulteração (2294255)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Windows Server 2008 R2, comunicada de forma privada, quando é utilizado como cluster de activação pós-falha partilhado. A vulnerabilidade poderia permitir a adulteração de dados nas partilhas administrativas de discos de cluster de activação pós-falha. Por predefinição, os servidores Windows Server 2008 R2 não são afectados por esta vulnerabilidade. Esta vulnerabilidade só se aplica a discos de cluster utilizados num cluster de activação pós-falha.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Moderada</a><br />
Adulteração</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Índice de possibilidade de exploração  
-------------------------------------
  
<span></span>
A tabela que se segue fornece uma avaliação da possibilidade de exploração para cada uma das vulnerabilidades abordadas este mês. As vulnerabilidades encontram-se listadas por ordem decrescente de nível de avaliação da possibilidade de exploração e, depois, por ID de CVE. Apenas são incluídas as vulnerabilidades às quais foi atribuída uma classificação de gravidade Crítica ou Importante nos boletins.
  
**Como utilizar esta tabela?**
  
Utilize esta tabela para saber mais sobre a probabilidade de códigos de exploração funcionais serem lançados no espaço de 30 dias após o lançamento do boletim de segurança, para cada uma das actualizações de segurança que poderá ter de instalar. Deverá rever cada avaliação em baixo, conforme a sua configuração específica, para dar prioridade à sua implementação. Para obter mais informações sobre o significado destas classificações e sobre como elas são estabelecidas, consulte o [Índice de Possibilidade de Exploração da Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                            | ID de CVE                                                                        | Avaliação do índice de possibilidade de exploração                                                               | Notas Principais                                                                                                                                                                                                        |  
|-----------------------------------------------------------|--------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-083](http://go.microsoft.com/fwlink/?linkid=190553) | Vulnerabilidade de Validação COM                                                     | [CVE-2010-1263](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1263) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-076](http://go.microsoft.com/fwlink/?linkid=194560) | Vulnerabilidade de Excesso de Número Inteiro em Tipos de Letra OpenType Incorporados | [CVE-2010-1883](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1883) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | O ASLR nos sistemas operativos mais recentes torna a exploração mais difícil                                                                                                                                            |  
| [MS10-078](http://go.microsoft.com/fwlink/?linkid=201084) | Vulnerabilidade de Análise de Tipos de Letra OpenType                                | [CVE-2010-2740](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2740) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-078](http://go.microsoft.com/fwlink/?linkid=201084) | Vulnerabilidade de Validação de Tipos de Letra OpenType                              | [CVE-2010-2741](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2741) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-073](http://go.microsoft.com/fwlink/?linkid=201093) | Vulnerabilidade de Esquema de Teclado no Win32k                                      | [CVE-2010-2743](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2743) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | **Esta vulnerabilidade foi divulgada publicamente e está a ser explorada actualmente no ecossistema da Internet**                                                                                                       |  
| [MS10-073](http://go.microsoft.com/fwlink/?linkid=201093) | Vulnerabilidade de Classe de Janelas no Win32k                                       | [CVE-2010-2744](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2744) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | **Esta vulnerabilidade foi divulgada publicamente**                                                                                                                                                                     |  
| [MS10-082](http://go.microsoft.com/fwlink/?linkid=201098) | Vulnerabilidade de Memória Danificada no Windows Media Player                        | [CVE-2010-2745](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2745) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-081](http://go.microsoft.com/fwlink/?linkid=201086) | Vulnerabilidade de Sobrecarga na Área Dinâmica para Dados no Comctl32                | [CVE-2010-2746](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2746) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Sobrecarga de Pilha no Word                                       | [CVE-2010-3214](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3214) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Marcadores no Word                                                | [CVE-2010-3216](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3216) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-084](http://go.microsoft.com/fwlink/?linkid=201720) | Vulnerabilidade de Sobrecarga de Memória Intermédia em Mensagens LPC                 | [CVE-2010-3222](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3222) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | **Esta vulnerabilidade foi divulgada publicamente**                                                                                                                                                                     |  
| [MS10-075](http://go.microsoft.com/fwlink/?linkid=201722) | Vulnerabilidade de Utilização Após Libertação RTSP                                   | [CVE-2010-3225](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3225) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-077](http://go.microsoft.com/fwlink/?linkid=201704) | Vulnerabilidade no Compilador JIT do .NET Framework x64                              | [CVE-2010-3228](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3228) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade na Análise de Formatos de Ficheiros Excel                            | [CVE-2010-3232](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3232) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Memória Danificada em Subsequências de Fórmulas                   | [CVE-2010-3234](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3234) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Registo BIFF em Fórmulas                                          | [CVE-2010-3235](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3235) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Matriz Fora dos Limites                                           | [CVE-2010-3236](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3236) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Função de Futuro Negativo                                         | [CVE-2010-3238](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3238) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade na Análise Extra de Registo Fora dos Limites                         | [CVE-2010-3239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3239) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Memória Danificada Não Inicializada                               | [CVE-2010-3326](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3326) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Memória Danificada Não Inicializada                               | [CVE-2010-3328](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3328) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Memória Danificada Não Inicializada                               | [CVE-2010-3329](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3329) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Memória Danificada Não Inicializada                               | [CVE-2010-3331](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3331) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Ponteiro Não Inicializado no Word                                 | [CVE-2010-2747](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2747) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Verificação de Limite no Word                                     | [CVE-2010-2748](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2748) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Índice no Word                                                    | [CVE-2010-2750](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2750) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Valor de Retorno no Word                                          | [CVE-2010-3215](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3215) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Ponteiro no Word                                                  | [CVE-2010-3217](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3217) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Sobrecarga na Área Dinâmica para Dados no Word                    | [CVE-2010-3218](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3218) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Análise de Índice no Word                                         | [CVE-2010-3219](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3219) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Análise no Word                                                   | [CVE-2010-3220](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3220) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | Vulnerabilidade de Análise no Word                                                   | [CVE-2010-3221](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3221) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Excesso de Número Inteiro ao Analisar Registos no Excel           | [CVE-2010-3230](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3230) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Memória Danificada na Análise de Registo no Excel                 | [CVE-2010-3231](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3231) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade na Análise de Livros do Lotus 1-2-3                                  | [CVE-2010-3233](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3233) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade no Ponteiro de Registo para Unir Células                             | [CVE-2010-3237](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3237) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Registo de Matriz de Dados em Tempo Real                          | [CVE-2010-3240](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3240) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade de Escrita de Memória Fora dos Limites na Análise                    | [CVE-2010-3241](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3241) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Vulnerabilidade na Análise de Registos do Tipo Fantasma                              | [CVE-2010-3242](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3242) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                               |  
| [MS10-073](http://go.microsoft.com/fwlink/?linkid=201093) | Vulnerabilidade de Contagem de Referência no Win32k                                  | [CVE-2010-2549](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2549) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | **Esta vulnerabilidade foi divulgada publicamente**                                                                                                                                                                     |  
| [MS10-085](http://go.microsoft.com/fwlink/?linkid=201705) | Vulnerabilidade de Negação de Serviço no TLSv1                                       | [CVE-2010-3229](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3229) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | O impacto de segurança máximo é apenas negação de serviço                                                                                                                                                               |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Sanitização de HTML                                               | [CVE-2010-3243](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3243) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | O [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) também resolve esta vulnerabilidade. O impacto de segurança máximo é apenas divulgação de informações.                                                      |  
| [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) | Vulnerabilidade de Sanitização de HTML                                               | [CVE-2010-3243](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3243) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | O [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) também resolve esta vulnerabilidade. O impacto de segurança máximo é apenas divulgação de informações.                                                      |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Sanitização de HTML                                               | [CVE-2010-3324](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3324) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | O [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) também resolve esta vulnerabilidade. **Esta vulnerabilidade foi divulgada publicamente.** O impacto de segurança máximo é apenas divulgação de informações. |  
| [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) | Vulnerabilidade de Sanitização de HTML                                               | [CVE-2010-3324](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3324) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | O [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) também resolve esta vulnerabilidade. **Esta vulnerabilidade foi divulgada publicamente.** O impacto de segurança máximo é apenas divulgação de informações. |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Divulgação de Informações em Caracteres Especiais CSS             | [CVE-2010-3325](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3325) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | **Esta vulnerabilidade foi divulgada publicamente.** O impacto de segurança máximo é apenas divulgação de informações.                                                                                                  |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Vulnerabilidade de Divulgação de Informações Entre Domínios                          | [CVE-2010-3330](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3330) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | O impacto de segurança máximo é apenas divulgação de informações                                                                                                                                                        |
  
Localizações do Software Afectado e das Transferências  
------------------------------------------------------
  
<span></span>
As tabelas que se seguem apresentam uma lista dos boletins ordenados de acordo com as principais categorias de software e nível de gravidade.
  
**Como utilizar estas tabelas?**
  
Utilize estas tabelas para saber mais sobre as actualizações de segurança que poderá ter de instalar. Deverá rever cada programa ou componente de software listado, para confirmar se alguma das actualizações de segurança se aplica à sua instalação. Se alguma aplicação ou componente de software estiver na lista, é fornecida uma hiperligação para a actualização de software disponível e é também a apresentada a classificação da gravidade da actualização de software.
  
**Nota** Poderá ter que instalar diversas actualizações de segurança para a mesma vulnerabilidade. Reveja toda a coluna para cada identificador de boletim listado, para verificar quais as actualizações que tem que instalar, com base nos programas ou componentes que tem instalados no seu sistema.
  
#### Sistema Operativo Windows e Componentes

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="14">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
I**dentificador do** **Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de** **Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3b029696-cf98-4935-b3d6-846110aaa4bb)  
(Crítica)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c77ee103-7e97-44b2-bbf3-ee9f0de37fed)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=93580299-d764-417f-a7fa-ee441fea2bb3)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c3799399-ca72-4dec-a2a2-3571ad0b2f63)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3966d754-d298-4e4a-9ce6-8205accd2215)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0553fc7c-deed-4594-a133-d621551310dc)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=912a7c20-8177-4f65-b986-43fca6375ec1)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player série 9](http://www.microsoft.com/downloads/details.aspx?familyid=bbf153e7-e764-46a0-a33b-81b7288d346c)  
(Importante)  
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=bbf153e7-e764-46a0-a33b-81b7288d346c)  
(Importante)  
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=bbf153e7-e764-46a0-a33b-81b7288d346c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=211d95be-5630-4af5-85a7-c50268c475a9)  
(KB979687)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6049c879-b81a-4d10-b96b-b2837cb24834)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=22f46b3b-9be6-45ea-a639-9974324ce4bd)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d494535a-b68e-4242-af85-5fa62f631ffc)  
(Crítica)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ff9c65fe-437c-426d-9096-dd89ff7927fd)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=05413f6c-b4be-4892-b4b3-c54dd01fd95d)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=860ff738-205d-430e-b223-b333813fc590)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7fd7c675-0675-4a87-a709-edc47a30f1e2)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ad30596-bac6-4d48-8b15-0245960c443b)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6c651bca-adb1-4172-9714-cd5a6e5d2c2a)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=0663e0e8-c5d1-4cd2-b6d3-ff78fb56bba1)  
(Importante)  
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=474b5618-dfe6-40de-b59b-1fd61a05749e)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b6f0898-8f77-4ce1-9c96-2b17c496230b)  
(KB979687)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d690846c-5e0b-4216-84cd-d17e366dd16d)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=285627b9-242d-4247-a4c8-55dc89386b62)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f64af3cd-591d-4212-94a0-3bc9a4d9782a)  
(Importante)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=fbcf0e65-c9f4-47f8-b4fc-ae46a66ab339)  
(Importante)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9af37f62-5585-4ff5-9dd3-3fa0b148ae08)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b240b65-f3ca-465c-a606-b561999c1977)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8ef4378e-21ff-4290-96ba-e00a60f372d1)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f94763e7-b1db-4043-aa79-d5be1a42307d)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b2eb449-ad55-4dfb-a3c5-aac767de6f45)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=5479fd20-50d1-447a-8555-a98ce0723f71)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13c08ec0-53ae-4b85-b669-8c88f6089259)  
(KB979687)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b31e18b0-da9f-4b3b-82c6-603e08b3b241)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d220f04e-9dbb-4b6d-924a-23065b48b8b6)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=12c3b950-b955-4820-9b4c-5206deb0cd3e)  
(Importante)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=59a715a5-10ff-40e6-88e0-096c9b640799)  
(Importante)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c8052f0c-e62c-46c4-bb59-d515fa388ea8)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=70c9e826-b80b-4a20-82d2-8e52e5cca839)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a95c74b-cfd8-45b5-8887-777429d21745)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6fca5cab-7e11-4911-a6a8-f73f113b2963)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=54fc4bc6-f46c-447c-8307-afd8338e7ffb)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=a9515e69-c147-4810-8c5a-6cb94c398a95)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=02519f9e-e1c5-48a1-8420-01898c45ec01)  
(KB979687)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1d73f0f1-6ec8-4304-a20e-345d8b6c225a)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=de908137-33e0-4f23-b32b-cc1bdbcb349c)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=97b3f6dc-8df5-4c93-aaee-f191498c7ce4)  
(Importante)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ba194be9-24f9-4c62-9aa9-9e98c81ddba1)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=bd5878bb-f565-4303-afed-4e17b44a02f2)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=21637cd8-c75c-43b4-9948-be7be54af6bf)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e8f297e2-0dfd-421a-b598-a78199ad6baa)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=64f5c311-d74a-4665-9775-ac91c6885ed3)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1064bccb-3ce6-4a72-8788-56d8021bca91)  
(KB979687)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=8fad4f77-7c89-4684-b957-9c00ced248d3)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=873dea9d-44cc-4e16-8a6d-dca678ce3a80)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="14">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 e Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4f656d16-2a7e-4d18-8a5a-ebf8a1a10e2b)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=191c8388-f1ef-45b6-9f07-d5654a973abe)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a481825-d9ad-4a7c-aa89-f40fb9651961)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29c4afb1-227d-4572-b136-a78ef7e1df77)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e9f735ab-d995-4209-b2dc-197f53fdee0f)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=95ceafc6-e37a-4c77-b16e-c9c94a7d89bd)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=95e24a63-d21a-4756-a16e-17a977595396)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80c99d69-4b97-4af2-8f8e-f3b300a89a5a)<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dff92449-22ad-49a8-8b28-5295a8af5b8b)<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4af2f6e6-6905-498c-bfba-a565976b3365)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=75ca4e2c-b0ae-46f4-a0fc-616510c41a55)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=02c6260c-8e21-401a-992d-884c6ff7141d)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=adeb3036-62fa-4a29-b82f-ff4a50c05996)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=15d8f81b-97b0-43d9-b218-1cdd759cb2ec)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=880ad9a0-6ddd-41f4-a608-171d59a31b6a)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=738c8f70-b46a-4a59-bea6-078074a9c4db)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dfe7cd18-53a3-433e-9a33-bd96b04b4deb)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=277151a2-b74f-4da6-8203-e774af75e44c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b73951f2-a7eb-4c7c-bf60-fdcfee83574f)<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9d2261f-bd9a-4495-a2f1-3c3b2208b01e)<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8c56ba29-b2a8-47a8-a605-4c54c0a7fa7c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a12ff95-ea5c-4c48-96c5-9494eb8f9f0d)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0107dd61-7b3e-4fcf-9743-d9ae594b2278)\*\*  
(Importante)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ea5b7c86-3878-43a9-a4bc-12e04bfbd06e)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=50386655-982e-4126-8261-2c972d695bbd)\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4dff0ebe-ccba-4675-98ca-9903f1cb6763)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5f079b0-d8e1-47fe-b9dd-41eeb463a93c)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=67eb3a70-9ca7-4184-b9fe-cc3e66b1bf36)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd507e7a-4516-474b-8f33-7fa8fd2afa6d)\*\*<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a8c2358-36ea-4757-abfc-5bffcad0a872)\*\*<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0566915f-2a1b-474b-b5f1-e1a9cedd836a)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=952b3594-d980-45b1-8fa3-49403784afbf)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=139f3bb2-eefc-4cf4-9c15-de78f5a736c1)\*\*  
(Importante)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=71ecdb27-46aa-4db1-b86a-3268cda88632)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a6b2ae1d-9225-4495-8560-97860f87d7b4)\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)\*\*<sup>[1]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=da7905a9-9587-4184-8fca-ecc636a3b67e)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e88d9c5-eb57-4d39-a880-a478c5f286da)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=33a06f0e-81ab-445a-bc89-14350ebfe688)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b5f53faf-61e2-4b4e-8b85-c5e8f38e5c30)\*\*<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=612ab78c-1ff1-45d2-96cc-ae831fb0a563)\*\*<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=74ac2233-02ec-454c-8aa0-64b18071e16a)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=21128031-d935-4e2d-b001-c502a2d6022c)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=1a971fb2-7dc4-43bf-ae25-3a420bb1acf9)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a4e38a77-3835-47b3-bd86-6c039169abf5)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9096046-8c7a-450c-b8c5-6e9fb001e6cd)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76e46d08-22d9-4a0c-82cd-d2753d07efe6)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5efe55b0-d34d-4f00-98b2-cc0e9807a8b9)<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d30368cb-c6e8-403e-aaf6-425f96b6211e)<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2fff281a-2221-42a3-a2b7-07b5c5e66ae7)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2eca0c38-73f5-4f83-ab62-97f979716a1d)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="14">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[Nenhum](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 para sistemas de 32 bits
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6595770f-e580-4613-a83a-3b8ee4cc30f1)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=1a3953fe-ba48-4980-a65d-74e3b756d53c)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=f6cae091-e9f1-48e9-a035-4346b9c6fec6)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=b5b31499-d242-42bf-ac78-b787ffb4d602)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=bdff9057-381a-44e8-b093-84f07d8d7e3c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 12](http://www.microsoft.com/downloads/details.aspx?familyid=59a2ef36-9c32-488b-b5b1-30b5bcd83358)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=b0d46bc3-24db-4207-b6fc-46b8cc64f075)<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=4a422192-d7fa-47e5-9661-2c65eaefaf62)<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=d7a08a66-08b4-421c-afad-f2f367d4a9f0)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=f09fbc23-cb6b-4525-8e41-8c14e8d03de9)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ffe364ee-e2ae-466c-b727-14b1a976a860)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=5759d2a3-7f35-4fa1-8ab4-17145839fa26)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=35882477-4e0a-4783-a4b4-0f1ea3398360)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=c47e8b74-8cfe-42d9-9362-8786687c88ad)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=35a2b1a9-6dd6-4a7e-bc0a-b4fcffa06b28)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 12](http://www.microsoft.com/downloads/details.aspx?familyid=00176d56-8a93-4780-96fc-a7ab715e7291)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=2de197c0-6d9e-460e-9509-f337fac8ee85)<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=03665687-8fd4-4afd-ac33-5f6824f51df8)<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=50d27c23-5f69-40fa-b517-32c245009467)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=abc24826-b83a-4e01-be68-8e3a73c10494)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d8b563ce-5db1-4490-8a63-44833d55152b)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=b060c516-233a-4e1e-9237-698420e97b2f)\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=98e0c6ac-c30b-4d39-8ed9-1fe69e7644e5)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=25fff010-3abc-45e6-979e-21d2bae49418)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Media Player 12](http://www.microsoft.com/downloads/details.aspx?familyid=4cf0e3b1-4b72-4f99-b716-2489ea42ed72)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=70622d35-4877-4cbb-bdbf-7648dc1ea8ed)\*\*<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=1c2ff242-65e3-4d47-bfca-4db30f809ed8)\*\*<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=d356af2f-eadf-4bf2-82d1-efa0d01ac92d)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=e4d27aa6-9739-4e41-9536-5f0b8d26503c)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=1de12fdf-b439-4020-9313-a193d47dcfb2)\*  
(Moderada)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)\*\*<sup>[1]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bbaa9f46-8fc7-4c44-b38c-dc3d5210f63d)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=0ead2ed9-8b2f-496e-b7d1-3ad2b04be5cc)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=44080c75-036e-4bd0-914a-74ab72189ee3)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d0742526-b5ec-4658-82f1-c3680f33a790)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3cec2b70-f694-4c0d-bf82-96a4fd50675d)<sup>[1]</sup>
(KB979687)  
(Importante)  
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f478020b-0305-47d5-bcb2-0758f292db29)<sup>[1]</sup>
(KB979688)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=334d39e6-8e4c-4e83-94c1-1db3d636e865)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c1634278-5598-45e0-81c6-f18fb5ba54cf)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1c607c7d-6144-4a39-beea-a31b62085047)  
(Moderada)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
</table>
 
**Nota para o MS10-077**

<sup>[1]</sup>**.NET Framework 4.0 e .NET Framework 4.0 Client Profile afectados.** Os pacotes .NET Framework Redistributable versão 4 estão disponíveis em dois perfis: .NET Framework 4.0 e .NET Framework 4.0 Client Profile. O .NET Framework 4.0 Client Profile é um subconjunto do .NET Framework 4.0. A vulnerabilidade resolvida nesta actualização afecta o .NET Framework 4.0 e o .NET Framework 4.0 Client Profile. Para mais informações, consulte o artigo MSDN sobre Instalação do .NET Framework.

**Nota para o MS10-083**

<sup>[1]</sup>Nos casos em que ambos os pacotes de actualizações de segurança KB979687 e KB979688 estão disponíveis para o mesmo sistema operativo, os clientes devem instalar ambos os pacotes para estarem protegidos contra as vulnerabilidades descritas no boletim MS10-083.

**Notas para o Windows Server 2008 e Windows Server 2008 R2**

**\*Instalação Server** **Core afectada.** Esta actualização aplica-se, com a mesma classificação de gravidade, a edições suportadas do Windows Server 2008 ou Windows Server 2008 R2, conforme indicado, quer a instalação tenha sido efectuada ou não utilizando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam as edições suportadas do Windows Server 2008 como indicado, se estas tiverem sido instaladas usando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Suites e Software do Microsoft Office

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Conjuntos de Aplicações e Componentes do Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
<td style="border:1px solid black;">
[**MS10-080**](http://go.microsoft.com/fwlink/?linkid=200529)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f22d10fd-cb12-43e8-88d5-2116cf4317c4)  
(KB2328360)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ea859881-2cc5-407b-a394-5d00c5d9fd97)  
(KB2345017)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=172f3743-cdfa-42d7-aeb4-27ba0e4139f7)  
(KB2344911)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3d9a00b8-0f80-4d36-b92a-89b61350fb36)  
(KB2344893)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ccad4871-32f2-4982-a23e-9b5824397615)<sup>[1]</sup>
(KB2344993)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dc9b9af5-50b0-4a07-8923-a30fd5548760)<sup>[1]</sup>
(KB2345035)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (edições de 32 bits)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2010 (edições de 32 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=6c3b8690-e568-42ed-a858-0cbdd5ea3669)  
(KB2345000)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (edições de 64 bits)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2010 (edições de 64 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=f31a1f9b-02df-4a85-a7d1-7d1e31baa30f)  
(KB2345000)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office para Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
<td style="border:1px solid black;">
[**MS10-080**](http://go.microsoft.com/fwlink/?linkid=200529)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 para Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=464965fa-971a-49dd-bcee-c4d91fac86a9)  
(KB2422343)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=464965fa-971a-49dd-bcee-c4d91fac86a9)  
(KB2422343)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 para Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=abd05074-8ffc-41a4-a2f3-1d8047574552)  
(KB2422352)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=abd05074-8ffc-41a4-a2f3-1d8047574552)  
(KB2422352)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Conversor de Formato de Ficheiros Open XML para Mac
</td>
<td style="border:1px solid black;">
[Conversor de Formato de Ficheiros Open XML para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5c759c46-ead3-44ea-b7c8-a308b3140d2e)  
(KB2422398)  
(Importante)
</td>
<td style="border:1px solid black;">
[Conversor de Formato de Ficheiros Open XML para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5c759c46-ead3-44ea-b7c8-a308b3140d2e)  
(KB2422398)  
(Importante)
</td>
</tr>
<tr>
<th colspan="3">
Outro Software Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
<td style="border:1px solid black;">
[**MS10-080**](http://go.microsoft.com/fwlink/?linkid=200529)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=1cb5ab02-074d-4877-b378-7058959705ae)  
(KB2345009)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Excel Viewer Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a833a94a-2dc0-4864-9c14-e196dc54c5a7)  
(KB2345088)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=553d28ae-c352-4985-97c3-e5038414be45)  
(KB2345043)  
(Importante)
</td>
<td style="border:1px solid black;">
[Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7391ec2f-12c9-483c-91d8-e3ec5754da1c)  
(KB2344875)  
(Importante)
</td>
</tr>
</table>
 
**Notas para o MS10-079**

<sup>[1]</sup>Para o Microsoft Word 2007 Service Pack 2, para além do pacote de actualização de segurança KB2344993, os clientes têm também de instalar a actualização de segurança para o Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2 (KB2345043) para estarem protegidos contra as vulnerabilidades descritas no boletim MS10-079.

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

**Nota para o MS10-080**

<sup>[1]</sup>Para o Microsoft Office Excel 2007 Service Pack 2, para além do pacote de actualização de segurança KB2345035, os clientes têm também de instalar a actualização de segurança para o Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2 (KB2344875) para estarem protegidos contra as vulnerabilidades descritas no boletim MS10-080.

#### Software Microsoft Server

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft SharePoint Services e Microsoft SharePoint Foundation
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-072**](http://go.microsoft.com/fwlink/?linkid=202016)
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows SharePoint Services 3.0
</td>
<td style="border:1px solid black;">
[Microsoft Windows SharePoint Services 3.0 Service Pack 2 (versões de 32 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=12fd97a9-6fb8-4b65-a497-a56587f114e1)  
(KB2345304)  
(Importante)  
[Microsoft Windows SharePoint Services 3.0 Service Pack 2 (versões de 64 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=58d1e91d-a037-485d-a6d9-80fbf403b108)  
(KB2345304)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Foundation 2010](http://www.microsoft.com/downloads/details.aspx?familyid=fc146fcb-c2cb-4860-a0cd-4b09fa3f44eb)  
(KB2345322)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="3">
Microsoft SharePoint e Microsoft Groove Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-072**](http://go.microsoft.com/fwlink/?linkid=202016)
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (edições de 32 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=aee3f2de-ccf3-4d32-b468-eede4e8afcd4)<sup>[1]</sup>
(KB2345212)  
(Importante)  
[Microsoft Office SharePoint Server 2007 Service Pack 2 (edições de 64 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=e5e60751-242a-4fdb-9852-6d94050d3d0e)<sup>[1]</sup>
(KB2345212)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Groove Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Groove Server 2010](http://www.microsoft.com/downloads/details.aspx?familyid=e032aef8-dd30-41c6-99bb-8cf0491451cc)  
(KB2346298)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office Web Apps
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-072**](http://go.microsoft.com/fwlink/?linkid=202016)
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps
</td>
<td style="border:1px solid black;">
[Microsoft Office Web Apps](http://www.microsoft.com/downloads/details.aspx?familyid=8fb56eb9-9601-4c1e-905a-9fe4802b2c8d)  
(KB2346411)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Web Apps](http://www.microsoft.com/downloads/details.aspx?familyid=8fb56eb9-9601-4c1e-905a-9fe4802b2c8d)<sup>[2]</sup>
(KB2346411)  
(Importante)  
[Microsoft Word Web App](http://www.microsoft.com/downloads/details.aspx?familyid=13b24264-ec3d-44e8-81e3-82ac767defd3)<sup>[2]</sup>
(KB2345015)  
(Importante)
</td>
</tr>
</table>
 
**Nota para o MS10-072**

<sup>[1]</sup>Para as edições suportadas do Microsoft SharePoint Server 2007, para além do pacote de actualização de segurança KB2345212, os clientes têm também de instalar a actualização de segurança para o Microsoft Windows SharePoint Services 3.0 (KB2345304) para estarem protegidos contra as vulnerabilidades descritas no boletim MS10-072.

**Notas para o MS10-079**

<sup>[2]</sup>Para as Microsoft Office Web Apps, os clientes terão de instalar ambas as actualizações de segurança KB2346411 e KB2345015 para estarem protegidos contra as vulnerabilidades descritas no boletim MS10-079.

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

Orientações e Ferramentas de Detecção e Implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para obter mais informações, visite o [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem na opção para obter as actualizações de segurança mais recentes.

As actualizações de segurança estão disponíveis no [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) e no [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). As actualizações de segurança estão também disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".

Por fim, as actualizações de segurança podem ser transferidas a partir do [Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). O Catálogo do Microsoft Update permite pesquisar conteúdos disponibilizados através do Windows Update e do Microsoft Update, incluindo actualizações de segurança, controladores e service packs. Utilizando o número do boletim de segurança para pesquisar (por exemplo, "MS07-036"), pode adicionar todas as actualizações aplicáveis ao seu cesto (incluindo diferentes idiomas para uma actualização) e transferi-las para uma pasta à sua escolha. Para obter mais informação sobre o Catálogo do Microsoft Update, consulte as [Perguntas Mais Frequentes sobre o Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Orientações de detecção e implementação**

A Microsoft fornece orientações sobre detecção e implementação de actualizações de segurança. Estas orientações contêm recomendações e informação que podem auxiliar os profissionais de TI a compreender como utilizar as diversas ferramentas para detecção e implementação de actualizações de segurança. Para obter mais informações, consulte o [Artigo 961747 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/961747).

**Microsoft Baseline Security Analyzer**

O Microsoft Baseline Security Analyzer (MBSA) permite aos administradores procurar actualizações de segurança em falta e comuns erros de configuração de segurança em sistemas locais e remotos. Para obter mais informações acerca do MBSA, visite o Web site do [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Ao utilizar os Windows Server Update Services (WSUS), os administradores podem implementar de forma rápida e fiável as actualizações críticas mais recentes e as actualizações de segurança para os sistemas operativos Microsoft Windows 2000 e posteriores, Office XP e posteriores, Exchange Server 2003 e SQL Server 2000 para o Microsoft Windows 2000 e sistemas operativos posteriores.

Para obter mais informações sobre como implementar esta actualização de segurança usando os Windows Server Update Services, visite o [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

O Microsoft Systems Management Server (SMS) fornece uma solução empresarial altamente configurável para gerir actualizações. O SMS permite aos administradores identificarem sistemas baseados no Windows que necessitem de actualizações de segurança e executar a implementação controlada dessas actualizações em toda a empresa, com um mínimo de incómodo para os utilizadores finais. O próximo lançamento do SMS, System Center Configuration Manager 2007, está agora disponível; consulte também [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Para mais informações sobre como os administradores podem utilizar o SMS 2003 para implementar actualizações de segurança, consulte [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Os utilizadores do SMS 2.0 também podem utilizar a Security Update Inventory Tool (SUIT) para ajudar a implementar actualizações de segurança. Para informações sobre o SMS, visite [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Nota** O SMS utiliza o Microsoft Baseline Security Analyzer para fornecer um suporte abrangente na detecção e implementação de actualizações dos boletins de segurança. Algumas actualizações de software poderão não ser detectadas por estas ferramentas. Nestes casos, os administradores podem utilizar as capacidades de inventário do SMS para fornecer actualizações a sistemas específicos. Para obter mais informações sobre este procedimento, consulte o artigo sobre como [Implementar actualizações de software utilizando a funcionalidade SMS Software Distribution](http://go.microsoft.com/fwlink/?linkid=33341). Algumas actualizações de segurança requerem direitos administrativos após o reinício do sistema. Os administradores podem utilizar a ferramenta Elevated Rights Deployment Tool (disponível no [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)) para instalar estas actualizações.

**Update Compatibility Evaluator e Application Compatibility Toolkit**

É frequente as actualizações utilizarem os mesmos ficheiros e configurações de registo necessários para a execução das aplicações. Isso pode dar origem a incompatibilidades e aumentar o tempo necessário para a implementação de actualizações de segurança. Pode simplificar o teste e a validação de actualizações do Windows relativamente às aplicações instaladas com os componentes do [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) incluído no [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

O Application Compatibility Toolkit (ACT) contém as ferramentas e documentação necessárias para avaliar e atenuar questões de compatibilidade da aplicação antes de implementar o Microsoft Windows Vista, uma Actualização do Windows, uma Actualização de Segurança da Microsoft ou uma nova versão do Windows Internet Explorer no seu ambiente.

### Outras informações

#### Ferramenta de Remoção de Software Malicioso Windows

A Microsoft publicou uma versão actualizada da Ferramenta de Remoção de Software Malicioso para o Microsoft Windows no Windows Update, no Microsoft Update, no Windows Server Update Services e no Centro de Transferências.

#### Actualizações não relacionadas com segurança, de elevada prioridade, no MU, WU e WSUS

Para obter informações sobre publicações não relacionadas com segurança no Windows Update e Microsoft Update, consulte:

-   [Artigo 894199 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/894199): Descrição das alterações de conteúdo do Software Update Services e Windows Server Update Services. Inclui todos os conteúdos do Windows.
-   [Actualizações de Meses Anteriores para o Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Apresenta todas as actualizações novas, revistas e relançadas para produtos Microsoft para além do Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

Para melhorar as protecções de segurança dos clientes, a Microsoft fornece informações sobre as vulnerabilidades aos principais fornecedores de software de segurança antes de cada publicação mensal de actualizações de segurança. Os fornecedores de software de segurança podem então utilizar estas informações sobre as vulnerabilidades para assegurar protecções actualizadas aos clientes através do seu software ou dispositivos de segurança, tais como antivírus, sistemas de detecção de intrusos com base na rede ou sistemas de prevenção de intrusões com base no anfitrião. Para determinar se as protecções activas estão disponíveis nos fornecedores de software de segurança, visite os Web sites de protecções activas disponibilizados pelos parceiros do programa, indicados na lista de [parceiros do Microsoft Active Protections Program (MAPP)](http://www.microsoft.com/security/msrc/mapp/partners.mspx).

#### Estratégias e comunidades de segurança

**Estratégias de Gestão de Actualizações**

As [Orientações de Segurança para Gestão de Actualizações](http://go.microsoft.com/fwlink/?linkid=21168) fornecem informações adicionais referentes a recomendações de melhores práticas da Microsoft para a aplicação de actualizações de segurança.

**Obter Outras Actualizações de Segurança**

Estão disponíveis actualizações para outros problemas de segurança nas seguintes localizações:

-   As actualizações de segurança estão disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".
-   As actualizações para plataformas de consumidor estão disponíveis no [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Pode obter as actualizações de segurança oferecidas no Windows Update este mês no ficheiro de imagem de CD em formato ISO com as informações de segurança e críticas no Centro de Transferências. Para obter mais informações, consulte o [Artigo 913086 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/913086).

**IT Pro Security Community**

Aprenda a melhorar a segurança, optimize a sua infra-estrutura informática e participe em tópicos de segurança juntamente com outros profissionais de informática no Web site [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Agradecimentos

A Microsoft [agradece](http://go.microsoft.com/fwlink/?linkid=21127) às seguintes entidades por trabalharem connosco para proteger os clientes:

-   [Sirdarckcat](http://www.sirdarckcat.net/), da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS10-071
-   Mario Heiderich, por fornecer informações sobre uma questão descrita no boletim MS10-071
-   Takehiro Takahashi, da [IBM ISS X-Force](http://www.iss.net/), por fornecer informações sobre uma questão descrita no boletim MS10-071
-   [Peter Vreugdenhil](http://vreugdenhilresearch.nl), a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [Tipping Point](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-071
-   Damián Frizza, da [Core Security Technologies](http://www.coresecurity.com/), por fornecer informações sobre uma questão descrita no boletim MS10-071
-   Aldwin Saugere e Radoslav Vasilev, da [Cigital](http://www.cigital.com/), por fornecerem informações sobre uma questão descrita no boletim MS10-071
-   Rodrigo Rubira Branco, do Centro de Investigação IPS da [Check Point](http://www.checkpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-071
-   [Sirdarckcat](http://www.sirdarckcat.net/), da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS10-072
-   Mario Heiderich, por fornecer informações sobre uma questão descrita no boletim MS10-072
-   Sergey Golovanov, Alexander Gostev, Maxim Golovkin e Alexey Monastyrsky, da [Kaspersky Lab](http://www.kaspersky.com), e Vitaly Kiktenko e Alexander Saprykin, da [Design and Test Lab](http://www.dnt-lab.com), por fornecerem informações sobre uma questão descrita no boletim MS10-073
-   Eric Chien, da [Symantec](http://www.symantec.com/index.jsp), por fornecer informações sobre uma questão descrita no boletim MS10-073
-   Tarjei Mandt, da [Norman](http://www.norman.com), por trabalhar connosco numa questão descrita no boletim MS10-073
-   Carsten H. Eiram, da [Secunia](http://secunia.com/), por trabalhar connosco numa questão descrita no boletim MS10-074
-   Oleksandr Mirosh, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [Tipping Point](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-075
-   Sebastian Apelt, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/)da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-076
-   Ivan Fratric, por fornecer informações através da [iSIGHT Partners Global Vulnerability Partnership](https://gvp.isightpartners.com/), sobre uma questão descrita no boletim MS10-076
-   Jeroen Frijters, da [Sumatra](http://www.sumatra.nl/), por fornecer informações sobre uma questão descrita no boletim MS10-077
-   Sebastian Apelt, da [siberas](http://www.siberas.de/), por fornecer informações sobre uma questão descrita no boletim MS10-078
-   Diego Juarez, da [Core Security Technologies](http://www.coresecurity.com/), por fornecer informações sobre uma questão descrita no boletim MS10-078
-   Chaouki Bekrar, da [Equipa de Investigação de Vulnerabilidades da VUPEN](http://www.vupen.com/), por fornecer informações sobre dez questões descritas no boletim MS10-079
-   Nicolas Joly, da [Equipa de Investigação de Vulnerabilidades da VUPEN](http://www.vupen.com/), por fornecer informações sobre uma questão descrita no boletim MS10-079
-   Alin Rad Pop, da [Secunia Research](http://secunia.com/), por fornecer informações sobre uma questão descrita no boletim MS10-079
-   Alin Rad Pop, da [Secunia](http://secunia.com/), por fornecer informações sobre duas questões descritas no boletim MS10-080
-   Chaouki Bekrar, da [Equipa de Investigação de Vulnerabilidades da VUPEN](http://www.vupen.com/), por fornecer informações sobre dez questões descritas no boletim MS10-080
-   Omair, por fornecer informações sobre uma questão descrita no boletim MS10-080
-   Carsten H. Eiram, da [Secunia](http://secunia.com/), por fornecer informações sobre duas questões descritas no boletim MS10-080
-   Krystian Kloskowski (h07), a trabalhar com a [Secunia](http://secunia.com/), por fornecer informações sobre uma questão descrita no boletim MS10-081
-   SkyLined, da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS10-082
-   HD Moore, da [Rapid7](http://www.rapid7.com/), por fornecer informações sobre uma questão descrita no boletim MS10-083
-   David Dewey, da [IBM ISS X-Force](http://www.iss.net/), e Ryan Smith, da [Accuvant](http://www.accuvant.com/), anteriormente [VeriSign iDefense Labs](http://labs.idefense.com/), por trabalharem connosco nas alterações a nível da protecção defensiva profunda no boletim MS10-083
-   [Mu Test Suite Team](http://www.mudynamics.com/products/mu-test-suite.html), da [Mu Dynamics](http://www.mudynamics.com/), por fornecer informações sobre uma questão descrita no boletim MS10-085

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre as opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para obter mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (12 de Outubro de 2010): Publicação do Resumo dos Boletins.
-   V1.1 (13 de Outubro de 2010): Alteração da classificação de gravidade da vulnerabilidade para o Windows Server 2008 e Windows Server 2008 R2 para Importante no boletim MS10-077. Corrigida também, no boletim MS10-082, a ligação de transferência para o Windows Media Player 11 no Windows XP Professional x64 Edition Service Pack 2.
-   V 2.0 (18 de Outubro de 2010): Para o MS10-085, foi alterada a descrição do Resumo Executivo para clarificar que a vulnerabilidade pode ser explorada em sistemas afectados que estejam configurados para receber tráfego de rede SSL. Trata-se de uma alteração informativa apenas. Os clientes que já tenham actualizado os seus sistemas com sucesso, incluindo clientes com as actualizações automáticas activadas, não necessitam de efectuar qualquer acção. Os clientes que não tenham instalado previamente esta actualização podem necessitar de reavaliar se os seus sistemas necessitam desta actualização.
-   V3.0 (14 de Dezembro de 2010): Revisão deste Resumo dos Boletins para anunciar o seguinte: Para o MS10-077, há novos pacotes de actualização para o .NET Framework 4.0 para corrigir uma questão na configuração que poderia interferir com a instalação bem sucedida de outras actualizações e/ou produtos. Os clientes que já tenham aplicado esta actualização com sucesso não necessitam de efectuar qualquer acção. Para o MS10-083, foi disponibilizada uma actualização adicional para o Windows Vista Service Pack 2 (KB979688) e Windows Server 2008 Service Pack 2 (KB979688) para utilizadores que instalaram o Windows Search 4.0 no Windows Vista Service Pack 1 ou Windows Server 2008, que depois instalaram a actualização de segurança oferecida em KB2405882 e que depois migraram para o Windows Vista Service Pack 2 ou Windows Server 2008 Service Pack 2. A nova actualização está disponível no [Artigo 2405882 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/2405882).
-   V4.0 (22 de Fevereiro de 2011): Para o MS10-077, foi anunciada uma alteração de detecção que agora oferece os pacotes de actualização do Microsoft .NET Framework 4.0 a clientes que instalaram o Microsoft .NET Framework 4.0 depois de terem instalado o Windows 7 para sistemas baseados em x64 Service Pack 1, Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1 ou Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1. Os clientes que já tenham aplicado esta actualização com sucesso não necessitam de efectuar qualquer acção.
-   V4.1 (26 de Outubro de 2011): Para MS10-077, corrigida a aplicabilidade da instalação Server Core para o .NET Framework 4 no Windows Server 2008 R2 para sistemas baseados em x64.

*Built at 2014-04-18T01:50:00Z-07:00*
