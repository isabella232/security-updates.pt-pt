---
TOCTitle: 'MS10-FEB'
Title: Resumo dos Boletins de Segurança Microsoft de Fevereiro 2010
ms:assetid: 'ms10-feb'
ms:contentKeyID: 61235156
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms10-feb(v=Security.10)'
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Fevereiro 2010
============================================================

Data de publicação: 9 de fevereiro de 2010 | Updated: 10 de fevereiro de 2010

**actualizada:** 1.1

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Fevereiro de 2010.

Com a publicação dos boletins de Fevereiro de 2010, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 4 de Fevereiro de 2010. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 10 de Fevereiro de 2010, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o webcast de boletins de segurança de Fevereiro](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032427679&culture=en-us). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

A Microsoft também fornece informações para ajudar os clientes a dar prioridade às actualizações de segurança mensais com quaisquer actualizações de elevada prioridade não relacionadas com segurança que sejam lançadas no mesmo dia que as actualizações de segurança mensais. Consulte a secção: **Outras informações**.

### Informação do Boletim

Resumos Executivos
------------------

<span></span>
A tabela seguinte resume os boletins de segurança para este mês, por ordem de gravidade.

Para obter mais informações sobre o software afectado, consulte a secção seguinte, **Localizações do Software Afectado e das Transferências**.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Identificação do Boletim</th>
<th style="border:1px solid black;" >Título do Boletim e Resumo Executivo</th>
<th style="border:1px solid black;" >Classificação de Gravidade Máxima e Impacto da Vulnerabilidade</th>
<th style="border:1px solid black;" >Requisito de Reinício</th>
<th style="border:1px solid black;" >Software Afectado</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=178850">MS10-006</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades em Cliente SMB Poderiam Permitir Execução Remota de Código (978251)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades no Microsoft Windows, comunicadas de forma privada. As vulnerabilidades poderiam permitir execução remota de código se um intruso enviasse uma resposta SMB especialmente concebida para o efeito a um pedido SMB iniciado pelo cliente. Para explorar estas vulnerabilidades, um intruso teria de convencer o utilizador a iniciar uma ligação SMB a um servidor SMB malicioso.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179067">MS10-007</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Processador da Shell do Windows Poderia Permitir Execução Remota de Código (975713)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade, comunicada de forma privada, no Microsoft Windows 2000, Windows XP e Windows Server 2003. As restantes versões do Windows não são afectadas por esta actualização de segurança. A vulnerabilidade poderia permitir a execução remota de código se uma aplicação, tal como um browser da Web, passasse dados especialmente concebidos para o efeito à função da API ShellExecute através do Processador da Shell do Windows.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179106">MS10-008</a></td>
<td style="border:1px solid black;"><strong>Actualização de Segurança Cumulativa de Kill Bits do ActiveX (978262)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade em software Microsoft, comunicada de forma privada. Esta actualização de segurança está classificada como Crítica para todas as edições suportadas do Microsoft Windows 2000 e Windows XP, Importante para todas as edições suportadas do Windows Vista e Windows 7, Moderada para todas as edições suportadas do Windows Server 2003 e Baixa para todas as edições suportadas do Windows Server 2008 e Windows Server 2008 R2.<br />
<br />
A vulnerabilidade poderia permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito que instanciasse um controlo ActiveX com o Internet Explorer. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. Esta actualização inclui também kill bits para quatro controlos ActiveX de outros fornecedores.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=167190">MS10-009</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades de TCP/IP no Windows Poderiam Permitir Execução Remota de Código (974145)</strong><br />
<br />
Esta actualização de segurança resolve quatro vulnerabilidades no Microsoft Windows, comunicadas de forma privada. A mais grave destas vulnerabilidades poderia permitir a execução remota de código se fossem enviados pacotes especialmente concebidos para o efeito a um computador com o IPv6 activado. Um intruso poderia tentar explorar a vulnerabilidade criando pacotes ICMPv6 especialmente concebidos para o efeito e enviando-os a um sistema com o IPv6 activado. Esta vulnerabilidade apenas pode ser explorada se o intruso tiver ligação activa.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítico</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=167321">MS10-013</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft DirectShow Poderia Permitir Execução Remota de Código (977935)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft DirectShow, comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um utilizador abrisse um ficheiro AVI especialmente concebido para o efeito. Um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=178812">MS10-003</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft Office (MSO) Poderia Permitir Execução Remota de Código (978214)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Office, comunicada de forma privada, que poderia permitir execução remota de código se um utilizador abrisse um ficheiro Office especialmente concebido para o efeito. Um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163639">MS10-004</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft Office PowerPoint Poderiam Permitir Execução Remota de Código (975416)</strong><br />
<br />
Esta actualização de segurança resolve seis vulnerabilidades no Microsoft Office PowerPoint, comunicadas de forma privada. As vulnerabilidades poderiam permitir a execução remota de código se um utilizador abrisse um ficheiro PowerPoint especialmente concebido para o efeito. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179066">MS10-010</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Windows Server 2008 Hyper-V Poderia Permitir Negação de Serviço (977894)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade, comunicada de forma privada, no Windows Server 2008 Hyper-V e no Windows Server 2008 R2 Hyper-V. A vulnerabilidade poderia permitir negação de serviço se uma sequência mal formada de instruções da máquina fosse executada por um utilizador autenticado numa das máquinas virtuais convidadas que seja alojada pelo Hyper-V Server. Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente numa máquina virtual convidada para explorar esta vulnerabilidade. A vulnerabilidade não poderia ser explorada remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Negação de Serviço</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179798">MS10-011</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Windows Client/Server Run-time Subsystem Poderia Permitir Elevação de Privilégios (978037)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade, comunicada de forma privada, no Microsoft Windows Client/Server Run-time Subsystem (CSRSS) no Microsoft Windows 2000, Windows XP e Windows Server 2003. As restantes versões do Windows não são afectadas. A vulnerabilidade poderia permitir elevação de privilégios se um intruso iniciasse sessão no sistema e iniciasse uma aplicação especialmente concebida para continuar a execução depois de o intruso terminar sessão. Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar esta vulnerabilidade. A vulnerabilidade não pode ser explorada por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=155976">MS10-012</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Servidor SMB Poderiam Permitir Execução Remota de Código (971468)</strong><br />
<br />
Esta actualização de segurança resolve várias vulnerabilidades no Microsoft Windows, comunicadas de forma privada. A mais grave destas vulnerabilidades poderia permitir a execução remota de código, se um intruso criasse um pacote SMB especialmente concebido para o efeito e o enviasse a um sistema afectado. Os procedimentos recomendados em relação à utilização de firewalls e as predefinições padrão de uma firewall podem ajudar a proteger as redes de ataques provenientes do exterior do perímetro da empresa que poderiam tentar explorar estas vulnerabilidades.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=181196">MS10-014</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Kerberos Poderia Permitir Negação de Serviço (977290)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir uma negação de serviço se um pedido de renovação de permissão especialmente concebido para o efeito fosse enviado para o domínio Kerberos do Windows a partir de um utilizador autenticado num realm Kerberos fiável que não do Windows. A negação de serviço poderia persistir até que o controlador de domínio fosse reiniciado.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Negação de Serviço</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179062">MS10-015</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Kernel do Windows Poderiam Permitir Elevação de Privilégios (977165)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente e uma vulnerabilidade comunicada de forma privada no Microsoft Windows. As vulnerabilidades poderiam permitir elevação de privilégios se um intruso iniciasse sessão no sistema e executasse uma aplicação especialmente concebida para o efeito. Para explorar qualquer uma destas vulnerabilidades, o intruso tem de ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente. As vulnerabilidades não poderiam ser exploradas remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=180620">MS10-005</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft Paint Poderia Permitir Execução Remota de Código (978706)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Paint, comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um utilizador visualizasse um ficheiro de imagem JPEG especialmente concebido para o efeito utilizando o Microsoft Paint. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Moderada</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Índice de possibilidade de exploração  
-------------------------------------
  
<span></span>
A tabela que se segue fornece uma avaliação da possibilidade de exploração para cada uma das vulnerabilidades abordadas este mês. As vulnerabilidades encontram-se listadas por ordem decrescente de nível de avaliação da possibilidade de exploração e, depois, por ID de CVE.
  
**Como utilizar esta tabela?**
  
Utilize esta tabela para saber mais sobre a probabilidade de códigos de exploração funcionais serem lançados no espaço de 30 dias após o lançamento do boletim de segurança, para cada uma das actualizações de segurança que poderá ter de instalar. Deverá rever cada avaliação em baixo, conforme a sua configuração específica, para dar prioridade à sua implementação. Para obter mais informações sobre o significado destas classificações e sobre como elas são estabelecidas, consulte o [Índice de Possibilidade de Exploração da Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                                                   | ID de CVE                                                                        | Avaliação do índice de possibilidade de exploração                                                               | Notas principais                                                                                                                 |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-006](http://go.microsoft.com/fwlink/?linkid=178850) | Vulnerabilidade de Condição Race em Cliente SMB                                                             | [CVE-2010-0017](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0017) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | O vector de ataque remoto poderia permitir negação de serviço; o vector de ataque local poderia permitir elevação de privilégios |  
| [MS10-011](http://go.microsoft.com/fwlink/?linkid=179798) | Vulnerabilidade de Elevação Local de Privilégios no CSRSS                                                   | [CVE-2010-0023](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0023) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | O intruso e a vítima têm de iniciar sessão na mesma consola                                                                      |  
| [MS10-007](http://go.microsoft.com/fwlink/?linkid=179067) | Vulnerabilidade de Validação de URL                                                                         | [CVE-2010-0027](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0027) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | Vulnerabilidade de Sobrecarga na Área Dinâmica para Dados LinkedSlideAtom no PowerPoint                     | [CVE-2010-0030](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0030) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | Vulnerabilidade de Indexação de Matriz Inválida OEPlaceholderAtom 'placementId' no PowerPoint               | [CVE-2010-0031](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0031) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | Vulnerabilidade de Utilização Após Libertação OEPlaceholderAtom no PowerPoint                               | [CVE-2010-0032](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0032) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | Vulnerabilidade de Sobrecarga de Pilha de Registo TextBytesAtom no PowerPoint Viewer                        | [CVE-2010-0033](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0033) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | A vulnerabilidade afecta apenas o PowerPoint Viewer 2003                                                                         |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | Vulnerabilidade de Sobrecarga de Pilha de Registo TextCharsAtom no Office PowerPoint Viewer                 | [CVE-2010-0034](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0034) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | A vulnerabilidade afecta apenas o PowerPoint Viewer 2003                                                                         |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | Vulnerabilidade de Falta de Entropia na Autenticação NTLM no SMB                                            | [CVE-2010-0231](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0231) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-015](http://go.microsoft.com/fwlink/?linkid=179062) | Vulnerabilidade no Processador de Excepções do Kernel do Windows                                            | [CVE-2010-0232](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0232) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-003](http://go.microsoft.com/fwlink/?linkid=178812) | Vulnerabilidade de Sobrecarga de Memória Intermédia no Ficheiro MSO.DLL                                     | [CVE-2010-0243](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0243) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-013](http://go.microsoft.com/fwlink/?linkid=167321) | Vulnerabilidade de Sobrecarga na Área Dinâmica para Dados no DirectShow                                     | [CVE-2010-0250](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0250) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                        |  
| [MS10-006](http://go.microsoft.com/fwlink/?linkid=178850) | Vulnerabilidade de Corrupção de Conjunto em Cliente SMB                                                     | [CVE-2010-0016](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0016) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                        |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | Vulnerabilidade de Sobrecarga de Nomes de Caminho no SMB                                                    | [CVE-2010-0020](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0020) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                        |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | Vulnerabilidade de Corrupção de Memória no SMB                                                              | [CVE-2010-0021](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0021) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                        |  
| [MS10-005](http://go.microsoft.com/fwlink/?linkid=180620) | Vulnerabilidade de Excesso de Número Inteiro no MS Paint                                                    | [CVE-2010-0028](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0028) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | Um exploração bem sucedida exige uma interacção significativa por parte do utilizador                                            |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | Vulnerabilidade de Sobrecarga de Memória Intermédia no Processamento de Caminhos de Ficheiros no PowerPoint | [CVE-2010-0029](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0029) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                        |  
| [MS10-015](http://go.microsoft.com/fwlink/?linkid=179062) | Vulnerabilidade de Condição Livre e Dupla no Kernel do Windows                                              | [CVE-2010-0233](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0233) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                        |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | Vulnerabilidade de Anúncio do Router ICMPv6                                                                 | [CVE-2010-0239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0239) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | A exploração requer que um intruso tenha ligação activa para o anfitrião visado                                                  |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | Vulnerabilidade na Fragmentação de MDL de Cabeçalho                                                         | [CVE-2010-0240](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0240) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | A vulnerabilidade requer um controlador de rede de terceiros                                                                     |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | Vulnerabilidade de Informação de Encaminhamento ICMPv6                                                      | [CVE-2010-0241](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0241) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | A exploração requer que um intruso tenha ligação activa para o anfitrião visado                                                  |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | Vulnerabilidade no Apontador NULL no SMB                                                                    | [CVE-2010-0022](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0022) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                        |  
| [MS10-010](http://go.microsoft.com/fwlink/?linkid=179066) | Vulnerabilidade de Validação de Conjuntos de Instruções no Hyper-V                                          | [CVE-2010-0026](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0026) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | A vulnerabilidade permite a possibilidade apenas de condição de negação de serviço                                               |  
| [MS10-014](http://go.microsoft.com/fwlink/?linkid=181196) | Vulnerabilidade de Não Referência no Apontador NULL no Kerberos                                             | [CVE-2010-0035](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0035) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Apenas negação de serviço; exploração apenas possível em controladores de domínio em configurações não predefinidas              |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | Vulnerabilidade de Reconhecimento Selectivo de TCP/IP                                                       | [CVE-2010-0242](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0242) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                        |
  
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
</tr>
<tr>
<th colspan="12">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
Nenhum
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=80b49bab-6c2f-48a8-a901-ca3f76e4fe6b)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=92234237-a8eb-4ce4-bc5e-cd86feb7dbd3)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=543dc6a7-fa76-4ba9-81e4-25fdf2013548)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Filtro AVI](http://www.microsoft.com/downloads/details.aspx?familyid=ba110440-10ce-40a0-884a-8b9afd45a3e3)  
(KB977914)  
(Crítica)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=16787c93-2c95-4c13-8492-be1db9d18146)  
(KB975560)  
(Crítica)  
[Quartz no DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=59a8bc19-02bb-4800-bac1-464f59e1cb7b)<sup>[1]</sup>
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=456185b5-57d1-4fa5-a4a9-5b2006ede3ad)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=267ce982-54a0-418f-ad52-e4963610f714)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=56a9afba-a6ee-4fb9-ba85-e51d9f94de27)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=ed8ac6a5-c8bb-4ed4-8994-810e9a1863c3)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=e5861705-8f49-45cb-8a92-cf052ccf4134)  
(Moderada)
</td>
</tr>
<tr>
<th colspan="12">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nenhum
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 e Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f6c4472e-385c-4412-bda9-c2e615e50713)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b8e7bf17-a037-4200-9ae2-2280b19766a4)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7bcf3945-0552-478e-b7f3-bbca97dd1b5d)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Filtro AVI](http://www.microsoft.com/downloads/details.aspx?familyid=a9beb2bd-e5f6-43f9-bbcc-a2afee5e5ceb)  
(KB977914)  
(Crítica)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7ab53be3-3f42-4e61-a2bc-3ed41d8736ff)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b9234b40-1b1c-498b-90d4-0bff347b36ee)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8f7adee3-e68e-41b3-b835-d84691774f31)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e2b348f5-ec8d-4782-bb03-5de550adea77)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b2e70df6-7728-4fc3-8df7-8ddb9ba5202f)  
(Moderada)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63e15ff0-73b3-46c9-96f8-c18977d35a10)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b8d83f30-9cd7-4d6b-b2b9-65d0a483cb9c)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25ef97e8-e76e-44c2-953c-f94cbac552cf)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Filtro AVI](http://www.microsoft.com/downloads/details.aspx?familyid=dedc3010-a989-45f7-b9d4-f7079db3e572)  
(KB977914)  
(Crítica)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7543e819-cd36-4e89-9850-60f00c50999d)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1f83bf7a-e16c-404a-89bd-f65843938299)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=91ee57f2-81e5-49bd-bdfc-d3e385efc8a5)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e534d00c-6ddc-4eb3-9464-5db6e90afa3e)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8c4acc8-c2f4-41f7-9b32-e7bd791e0155)  
(Moderada)
</td>
</tr>
<tr>
<th colspan="12">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=feb8c145-7c30-45fa-a6f0-8b6453ddd521)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5cb2e203-18fb-4887-a1c9-289d86b8ba11)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29ff72f7-1663-4f35-a794-2dfe3c17b39c)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Filtro AVI](http://www.microsoft.com/downloads/details.aspx?familyid=cc5150d7-070e-4a87-9c02-d050a8cb2204)  
(KB977914)  
(Crítica)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=983c5484-6321-4765-97ec-8d42d42d1f70)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c8c4eec-255e-41d5-b1e6-f0204edcb46f)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d18cbc4-ac48-458c-8aa3-90708fd854ff)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=738e2fda-96fc-413d-a5c7-74b1fac1d6b3)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=defd8603-ed9b-42f9-a539-2b6a690e9575)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1efbe73-fc87-4e6a-8b36-81f125a27aec)  
(Moderada)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36d88c1b-814c-4371-9ed2-d4576f419fc3)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=90360537-9311-45e2-8047-9a971f90c3c3)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d4a97bb7-4f74-4884-9a6e-7a4df9c540fb)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Filtro AVI](http://www.microsoft.com/downloads/details.aspx?familyid=db13e99b-2f2a-4474-8d6e-271b025bd07f)  
(KB977914)  
(Crítica)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7dc20252-6091-407b-befc-c25e8f5d3fb0)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=de0186f6-27a2-4226-b8eb-f2912710f072)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d63c95e-311a-446f-8852-dffd217a89f6)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8ad539d-8191-4864-977b-ad4e31c04ba0)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9873c962-9d3d-46ef-b54b-2a50696fb6b2)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9143e435-f0d6-464b-9273-4d1f38f8ff3a)  
(Moderada)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=622442b0-cffe-4fc2-94a8-edff9d71ecd3)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d695ca9f-a1db-4c0f-94b6-7112861c28da)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b84f0be4-6d11-4b07-bb3c-2c76ae9ceea8)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Filtro AVI](http://www.microsoft.com/downloads/details.aspx?familyid=aec66173-e2c6-4c39-8d60-8fbef6d7b764)  
(KB977914)  
(Importante)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=b1a7533a-913f-4054-b579-489a257bae5f)  
(KB975560)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=87732f7a-9339-43bc-a4e8-3da849f35b70)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ee7f8cc4-f7fd-4dc7-808c-436204ee80cb)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d549c927-add7-4d83-bfc7-15dc35663dfb)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c3c21225-8534-4c7f-96b6-20a743dcea74)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ee603435-26af-4ab9-9f22-92734346dc0a)  
(Moderada)
</td>
</tr>
<tr>
<th colspan="12">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
Nenhum
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
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1902fc93-0f4b-4261-9da3-17d1931daf2e)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c897ddd-f441-41d4-b5b4-d794cfc96e6b)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71f03946-622c-4403-b94f-f6a3de18a8c3)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7130ce0f-df38-4c96-ac54-cdbff35f03e7)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=16494dac-553a-4de9-b751-0d6b51cb43f0)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2761c7b4-d472-4f00-949b-af3ebafdc08d)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c2f89b5-a3b3-42cd-857d-923fe8b8f1da)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f349f7aa-d020-4e0d-a35f-518a63ec92df)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=519815fd-707d-476f-9e29-7b03b7a17af5)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=de7b7c8f-bd0a-4e13-bd58-d95507a6274b)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cec582b3-e37f-448e-a5c3-6abdcee9e57c)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=38b40dab-6b4d-434b-9997-12ef70d6bbcc)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="12">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
[**Baixa**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=09e19263-18ba-495e-bcf7-719e957204a7)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a85b1bf-7427-47d0-9e1b-21dbe824a62c)\*\*  
(Baixo)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc451228-3de4-427c-b42f-91f204c708b8)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=5ac0a948-0bdc-4c10-9b88-16a5d7092e47)\*\*  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=597b2310-2cd8-4d0f-8248-781eb8b7450a)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=75327470-0f14-4cdd-bcb7-64684c61c267)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=21e87558-9bd2-4aa9-aaa5-7fd26a5b60e6)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=180c2313-5e3e-4d84-87cd-64048f51e0f6)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fde218c3-90ab-4664-852d-25ca55835054)\*\*  
(Baixo)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3a889152-5d7c-4a3e-b4f1-c6507b739ca0)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=362fea40-649b-4471-aad7-db29edd0ac10)\*\*  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3463a63c-e88a-4036-ab60-f84d4bf4191a)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=67119fb6-e517-46f4-ab0b-2351cdc3d670)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d0f8f81-fc10-450a-a653-06f89acba9fa)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0b93047d-f2c6-403b-9200-c251898bc1e0)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614eaf7e-95aa-4f8f-910c-1980e1f14d11)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b6e9451-df38-4626-bb1d-4fc160d7a40e)  
(Baixo)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1cd1882b-8e55-47ea-a82a-68bb59a500a7)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=effa638b-cfc1-4777-8219-7b433ed5e717)  
(KB975560)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f90fc0c8-babe-4224-be07-614ea7ddf102)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cd6b234b-8e96-4128-a77a-645a0882996a)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="12">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
Nenhum
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
Nenhum
</td>
<td style="border:1px solid black;">
Nenhum
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
Nenhum
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 para sistemas de 32 bits
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=a589431a-93dc-42cd-a74e-d9c1e3452fef)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=ec6d996f-dffa-45ad-9467-e96a4ac63e5f)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=4ec49aa2-81df-4e65-80da-6201394c4089)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=122fc003-0651-4ad2-a5c8-a21536defad8)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=66f14bb4-40fc-4ae3-9baf-429b7106cd91)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=3c1edcf8-d304-45c4-9818-1cd86383b3fe)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=b3265576-04c1-48b1-8ce9-128843c58cf5)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=a8a2519c-3b89-4987-9473-920adafc78cb)  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=3e096468-db6c-45c6-bee5-eaeaa63500b5)  
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
</tr>
<tr>
<th colspan="12">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
Nenhum
</td>
<td style="border:1px solid black;">
[**Baixa**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=ecb06350-47a7-48eb-825f-3e8f89c5ca8e)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=cda31c54-8b81-4185-a623-64480ad4b73c)\*\*  
(Baixo)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=a9811baa-1500-4c73-940b-57f8c5456891)\*\*  
(KB975560)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=3214b347-d901-4aac-85ce-676e4602de87)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=dc757b6d-f0f8-4e71-ab6f-1417233eedf9)\*  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=badd6cab-7738-4401-a68c-c15414388601)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=43fa4e26-160f-4aa3-a03d-b98a79666a18)  
(Baixo)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=2ed23bf5-6217-413c-a7ba-eccc82139d68)  
(KB975560)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d5b0b1eb-24f3-47ec-aba1-c1b95400189e)  
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
</tr>
</table>
 
**Nota para o MS10-013**

<sup>[1]</sup>A actualização para o DirectX 9.0 também se aplica ao DirectX 9.0a, DirectX 9.0b e DirectX 9.0c no Microsoft Windows 2000.

**Notas para o Windows Server 2008 e Windows Server 2008 R2**

**\*Instalação Server Core afectada.** Esta actualização aplica-se, com a mesma classificação de gravidade, a edições suportadas do Windows Server 2008 ou Windows Server 2008 R2, conforme indicado, quer a instalação tenha sido efectuada ou não utilizando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) e [Server Core para Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e do Windows Server 2008 R2; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 e Windows Server 2008 R2 como indicado, se estes tiverem sido instalados usando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) e [Server Core para Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e do Windows Server 2008 R2; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
Suites, Sistemas e Componentes do Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-003**](http://go.microsoft.com/fwlink/?linkid=178812)
</td>
<td style="border:1px solid black;">
[**MS10-004**](http://go.microsoft.com/fwlink/?linkid=163639)
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
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=47553f45-fa10-40e5-8267-9d42ff560a62)  
(KB977896)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cfc697b4-2ceb-4030-86c5-be9bc8bfd07c)  
(KB973143)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2291ae24-fa39-4ad8-a7d0-12726b68ad96)  
(KB976881)  
(Importante)
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office para Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-003**](http://go.microsoft.com/fwlink/?linkid=178812)
</td>
<td style="border:1px solid black;">
[**MS10-004**](http://go.microsoft.com/fwlink/?linkid=163639)
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
Microsoft Office 2004 para Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=7c985595-00c5-44b8-81c3-59d9967220f8)<sup>[1]</sup>
(KB979674)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=7c985595-00c5-44b8-81c3-59d9967220f8)<sup>[1]</sup>
(KB979674)  
(Importante)
</td>
</tr>
</table>
 
**Nota para Microsoft Office para Mac**

<sup>[1]</sup>Devido ao modelo de prestação de serviços cumulativo para o Microsoft Office 2004 para Mac, estas actualizações são idênticas.

Orientações e ferramentas de detecção e implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para mais informações, visite o [Centro de Gestão de Actualizações TechNet](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em Casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem na opção para obter as actualizações de segurança mais recentes.

As actualizações de segurança estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt) e no [Windows Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt). As actualizações de segurança estão também disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".

Finalmente, as actualizações de segurança podem ser transferidas a partir do [Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). O Catálogo do Microsoft Update permite pesquisar conteúdos disponibilizados através do Windows Update e do Microsoft Update, incluindo actualizações de segurança, controladores e service packs. Utilizando o número do boletim de segurança para pesquisar (por exemplo, "MS07-036"), pode adicionar todas as actualizações aplicáveis ao seu cesto (incluindo diferentes idiomas para uma actualização) e transferi-las para uma pasta à sua escolha. Para mais informação sobre o Catálogo do Microsoft Update, consulte as [Perguntas Mais Frequentes sobre o Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Nota** Desde 1 de Agosto de 2009, a Microsoft deixou de prestar suporte para o Office Update e a ferramenta Office Update Inventory Tool. Para continuar a obter as mais recentes actualizações para produtos Microsoft Office, utilize o [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt). Para mais informações, consulte [Acerca do Microsoft Office Update: Perguntas Mais Frequentes](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx).

**Orientações de detecção e implementação**

A Microsoft fornece orientações sobre detecção e implementação de actualizações de segurança. Estas orientações contêm recomendações e informação que podem auxiliar os profissionais de TI a compreender como utilizar as diversas ferramentas para detecção e implementação de actualizações de segurança. Para obter mais informações, consulte o [Artigo 961747 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/961747).

**Microsoft Baseline Security Analyzer**

O Microsoft Baseline Security Analyzer (MBSA) permite aos administradores procurar actualizações de segurança em falta e comuns erros de configuração de segurança em sistemas locais e remotos. Para obter mais informações acerca do MBSA, visite o Web site do [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Ao utilizar os Windows Server Update Services (WSUS), os administradores podem implementar de forma rápida e fiável as actualizações críticas mais recentes e as actualizações de segurança para os sistemas operativos Microsoft Windows 2000 e posteriores, Office XP e posteriores, Exchange Server 2003 e SQL Server 2000 para o Microsoft Windows 2000 e sistemas operativos posteriores.

Para mais informações sobre como implementar esta actualização de segurança usando os Windows Server Update Services, visite o [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

O Microsoft Systems Management Server (SMS) fornece uma solução empresarial altamente configurável para gerir actualizações. O SMS permite aos administradores identificarem sistemas baseados no Windows que necessitem de actualizações de segurança e executar a implementação controlada dessas actualizações em toda a empresa, com um mínimo de incómodo para os utilizadores finais. O próximo lançamento do SMS, System Center Configuration Manager 2007, está agora disponível; consulte também [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Para mais informações sobre como os administradores podem utilizar o SMS 2003 para implementar actualizações de segurança, consulte [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Os utilizadores do SMS 2.0 também podem utilizar a Security Update Inventory Tool (SUIT) para ajudar a implementar actualizações de segurança. Para informações sobre o SMS, visite [Microsoft Systems Management Server](http://www.microsoft.com/portugal/smserver/default.mspx).

**Nota** O SMS utiliza o Microsoft Baseline Security Analyzer para fornecer um suporte abrangente na detecção e implementação de actualizações dos boletins de segurança. Algumas actualizações de software poderão não ser detectadas por estas ferramentas. Nestes casos, os administradores podem utilizar as capacidades de inventário do SMS para fornecer actualizações a sistemas específicos. Para mais informações sobre este procedimento, veja o artigo sobre como [Implementar actualizações de software utilizando a funcionalidade SMS Software Distribution](http://go.microsoft.com/fwlink/?linkid=33341). Algumas actualizações de segurança requerem direitos administrativos após o reinício do sistema. Os administradores podem utilizar a ferramenta Elevated Rights Deployment Tool (disponível no [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)) para instalar estas actualizações.

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
-   As actualizações para plataformas de consumidor estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt).
-   Pode obter as actualizações de segurança oferecidas no Windows Update este mês no ficheiro de imagem de CD em formato ISO com as informações de segurança e críticas no Centro de Transferências. Para mais informações, consulte o [Artigo 913086 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/913086).

**IT Pro Security Community**

Aprenda a melhorar a segurança, optimize a sua infra-estrutura informática e participe em tópicos de segurança juntamente com outros profissionais de informática no Web site [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Agradecimentos

A Microsoft [agradece](http://go.microsoft.com/fwlink/?linkid=21127) às seguintes entidades por trabalharem connosco para proteger os clientes:

-   Damian Frizza, da [Core Security Technologies](http://www.coresecurity.com/), por fornecer informações sobre uma questão descrita no boletim MS10-003
-   Carsten Eiram, da [Secunia](http://secunia.com/), por fornecer informações sobre uma questão descrita no boletim MS10-004
-   Sean Larsson, da [VeriSign iDefense Labs](http://labs.idefense.com/), por fornecer informações sobre três questões descritas no boletim MS10-004
-   SkD, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-004
-   Cody Pierce, da [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-004
-   Tielei Wang, do ICST-ERCIS (Engineering Research Center of Info Security, Institute of Computer Science & Technology, Peking University/China), a trabalhar com a [Secunia](http://secunia.com/), por fornecer informações sobre uma questão descrita no boletim MS10-005
-   Laurent Gaffié, da [stratsec](http://www.stratsec.net/), por fornecer informações sobre duas questões descritas no boletim MS10-006
-   Brett Moore, a trabalhar com a [TippingPoint](http://www.tippingpoint.com/) e a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecer informações sobre uma questão descrita no boletim MS10-007
-   [Lostmon Lords](http://lostmon.blogspot.com/), por fornecer informações sobre uma questão descrita no boletim MS10-007
-   Shaun Colley, da [NGS Software](http://www.ngssoftware.com/), por fornecer informações sobre uma questão descrita no boletim MS10-008
-   Sumit Gwalani, Drew Hintz e Neel Mehta, da [Google Security Team](http://www.google.com/), por fornecerem informações sobre três questões descritas no boletim MS10-009
-   Jan Bottorff, por fornecer informações sobre uma questão descrita no boletim MS10-010
-   Matthew 'j00ru' Jurczyk e Gynvael Coldwind, da [Hispasec](http://www.hispasec.com/), por fornecerem informações sobre uma questão descrita no boletim MS10-011
-   Joshua Morin, da [Codenomicon](http://www.codenomicon.com/), por fornecer informações sobre uma questão descrita no boletim MS10-012
-   Florian Rienhardt, da [BSI](http://www.bsi.bund.de/), por fornecer informações sobre uma questão descrita no boletim MS10-012
-   Hernan Ochoa (Investigador / Consultor Independente de Segurança da Informação), por fornecer informações sobre uma questão descrita no boletim MS10-012
-   Investigador anónimo, a trabalhar com a [TippingPoint](http://www.tippingpoint.com/) e a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecer informações sobre uma questão descrita no boletim MS10-013
-   Tavis Ormandy, da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS10-015

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (9 de Fevereiro de 2010): Publicação do Resumo dos Boletins.
-   V1.1 (10 de Fevereiro de 2010) : Correcção dos requisitos de reinício para o boletim MS10-005.

*Built at 2014-04-18T01:50:00Z-07:00*
