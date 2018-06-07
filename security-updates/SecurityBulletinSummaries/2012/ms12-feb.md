---
TOCTitle: 'MS12-FEB'
Title: Resumo dos Boletins de Segurança Microsoft de Fevereiro de 2012
ms:assetid: 'ms12-feb'
ms:contentKeyID: 61235180
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms12-feb(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Fevereiro de 2012
===============================================================

Data de publicação: 14 de fevereiro de 2012

**actualizada:** 1.0

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Fevereiro de 2012.

Com a publicação dos boletins de segurança de Fevereiro de 2012, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 9 de Fevereiro de 2012. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 15 de Fevereiro de 2012, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o webcast de boletins de segurança de Fevereiro](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499501). Depois desta data, o webcast estará disponível mediante pedido. Para obter mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

A Microsoft também fornece informações para ajudar os clientes a dar prioridade às actualizações de segurança mensais com quaisquer actualizações não relacionadas com segurança que sejam lançadas no mesmo dia que as actualizações de segurança mensais. Consulte a secção: **Outras informações**.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238387">MS12-008</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades nos Controladores de Modo de Kernel do Windows Poderiam Permitir Execução Remota de Código (2660465)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada e uma vulnerabilidade divulgada publicamente no Microsoft Windows. A mais grave destas vulnerabilidades poderia permitir a execução remota de código se um utilizador visitasse um Web site com conteúdo especialmente concebido para o efeito ou se fosse executada localmente uma aplicação especialmente concebida para o efeito. Um intruso não conseguiria obrigar os utilizadores a visitarem um Web site malicioso. Em vez disso, um intruso teria de convencer os utilizadores a visitar o Web site, levando-os normalmente a clicar numa hiperligação presente numa mensagem de correio electrónico ou num programa de mensagens instantâneas, que levasse o utilizador para o Web site do intruso.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=236989">MS12-010</a></td>
<td style="border:1px solid black;"><strong>Actualização de Segurança Cumulativa para o Internet Explorer (2647516)</strong><br />
<br />
Esta actualização de segurança resolve quatro vulnerabilidades no Internet Explorer, comunicadas de forma privada. As vulnerabilidades mais graves poderiam permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer. Um intruso que conseguisse explorar qualquer uma destas vulnerabilidades com sucesso poderia obter os mesmos privilégios que o utilizador com sessão iniciada. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238617">MS12-013</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na Biblioteca de Runtime em C Poderia Permitir Execução Remota de Código (2654428)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro multimédia especialmente concebido para o efeito alojado num Web site ou enviado como anexo de correio electrónico. Um intruso que explorasse a vulnerabilidade com sucesso poderia obter os mesmos direitos que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235370">MS12-016</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no .NET Framework e no Microsoft Silverlight Poderiam Permitir Execução Remota de Código (2651026)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente e uma vulnerabilidade comunicada de forma privada no Microsoft. NET Framework e Microsoft Silverlight. As vulnerabilidades poderiam permitir a execução remota de código num sistema cliente se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando um browser da Web que pudesse executar Aplicações de Browser XAML (XBAPs) ou aplicações Silverlight. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft .NET Framework,<br />
Microsoft Silverlight</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238474">MS12-009</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Controlador de Função Auxiliar Poderiam Permitir Elevação de Privilégios (2645640)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades no Microsoft Windows, comunicadas de forma privada. As vulnerabilidades poderiam permitir elevação de privilégios se um intruso iniciasse sessão no sistema de um utilizador e executasse uma aplicação especialmente concebida para o efeito. Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar as vulnerabilidades.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238500">MS12-011</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft SharePoint Poderiam Permitir Elevação de Privilégios (2663841)</strong><br />
<br />
Esta actualização de segurança resolve três vulnerabilidades, comunicadas de forma privada, no Microsoft SharePoint e no Microsoft SharePoint Foundation. Estas vulnerabilidades poderiam permitir elevação de privilégios ou divulgação de informações se um utilizador clicasse num URL especialmente concebido para o efeito.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Software Microsoft Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=239941">MS12-012</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na Cor do Painel de Controlo Poderia Permitir Execução Remota de Código (2643719)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows comunicada publicamente. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro legítimo (como um ficheiro .icm ou .icc) localizado no mesmo directório que um ficheiro de biblioteca de hiperligação dinâmica (DLL) especialmente concebido. Um intruso que conseguisse explorar esta vulnerabilidade com êxito poderia obter os mesmos privilégios que o utilizador com sessão iniciada. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=239945">MS12-014</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Codec Indeo Poderia Permitir Execução Remota de Código (2661637)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows comunicada publicamente. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro legítimo (como um ficheiro .avi) localizado no mesmo directório que um ficheiro de biblioteca de hiperligação dinâmica (DLL) especialmente concebido. Um intruso que conseguisse explorar esta vulnerabilidade com êxito poderia executar código arbitrário em nome do utilizador com sessão iniciada. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Se um utilizador tiver sessão iniciada com direitos de utilizador administrativos, um intruso poderia obter controlo total sobre o sistema afectado. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238400">MS12-015</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft Visio Viewer 2010 Poderiam Permitir Execução Remota de Código (2663510)</strong><br />
<br />
Esta actualização de segurança resolve cinco vulnerabilidades no Microsoft Office, comunicadas de forma privada. As vulnerabilidades poderiam permitir a execução remota de código se um utilizador abrisse um ficheiro Visio especialmente concebido para o efeito. Um intruso que conseguisse explorar estas vulnerabilidades com sucesso poderia obter os mesmos privilégios que o utilizador com sessão iniciada. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Índice de possibilidade de exploração  
-------------------------------------
  
<span></span>
A tabela que se segue fornece uma avaliação da possibilidade de exploração para cada uma das vulnerabilidades abordadas este mês. As vulnerabilidades encontram-se listadas por ordem de identificação do boletim e, depois, de CVE. Apenas são incluídas as vulnerabilidades às quais foi atribuída uma classificação de gravidade Crítica ou Importante nos boletins.
  
**Como utilizar esta tabela?**
  
Utilize esta tabela para saber mais sobre a probabilidade de serem lançadas explorações por execução de código e negação de serviço no espaço de 30 dias após o lançamento do boletim de segurança, para cada uma das actualizações de segurança que poderá ter de instalar. Reveja cada uma das avaliações abaixo, conforme a sua configuração específica, para dar prioridade à sua implementação de actualizações deste mês. Para obter mais informações sobre o significado destas classificações e sobre como elas são estabelecidas, consulte o [Índice de Possibilidade de Exploração da Microsoft](http://technet.microsoft.com/security/cc998259.aspx).
  
Nas colunas abaixo, "Lançamento de Software Mais Recente" refere-se ao software em questão e "Lançamentos de Software Mais Antigos" refere-se a todos os lançamentos mais antigos do software em questão que são suportados, conforme listado nas tabelas de "Software Afectado" e "Software Não Afectado" do boletim.
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                                | ID de CVE                                                                         | Avaliação da Possibilidade de Exploração para o Lançamento de Software Mais Recente                       | Avaliação da Possibilidade de Exploração para o Lançamento de Software Mais Antigo                        | Avaliação da Possibilidade de Exploração da Negação de Serviço | Notas Principais                                                                                                |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|  
| [MS12-008](http://go.microsoft.com/fwlink/?linkid=238387) | Vulnerabilidade de Utilização Após Libertação de Esquema de Teclado                      | [CVE-2012-0154](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0154)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não Aplicável                                                  | (Nenhuma)                                                                                                       |  
| [MS12-008](http://go.microsoft.com/fwlink/?linkid=238387) | Vulnerabilidade de Violação de Acesso a GDI                                              | [CVE-2011-5046](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-5046)  | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Seria difícil criar código de exploração | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Seria difícil criar código de exploração | Permanente                                                     | Esta vulnerabilidade foi divulgada publicamente.                                                                |  
| [MS12-009](http://go.microsoft.com/fwlink/?linkid=238474) | Vulnerabilidade de Elevação de Privilégios no AfdPoll                                    | [CVE-2012-0148](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0148)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração          | Permanente                                                     | X64 é explorável, x86 não é.                                                                                    |  
| [MS12-009](http://go.microsoft.com/fwlink/?linkid=238474) | Vulnerabilidade de Elevação de Privilégios no Controlador de Função Auxiliar             | [CVE-2012-0149](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0149)  | Não afectado                                                                                              | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Permanente                                                     | Apenas é afectado o Windows Server 2003.                                                                        |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | Vulnerabilidade de Execução Remota de Código em Esquema de HTML                          | [CVE-2012-0011](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0011)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Temporário                                                     | (Nenhuma)                                                                                                       |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | Vulnerabilidade de Divulgação de Informações por Byte Nulo                               | [CVE-2012-0012](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0012)  | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração          | Não afectado                                                                                              | Não Aplicável                                                  | Trata-se de uma vulnerabilidade ao nível da divulgação de informações.                                          |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | Vulnerabilidade de Execução Remota de Código em Ficheiros VML                            | [CVE-2012- 0155](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0155) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não afectado                                                                                              | Temporário                                                     | (Nenhuma)                                                                                                       |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Vulnerabilidade de XSS no inplview.aspx                                                  | [CVE-2012-0017](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0017)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não afectado                                                                                              | Não Aplicável                                                  | (Nenhuma)                                                                                                       |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Vulnerabilidade de XSS no themeweb.aspx                                                  | [CVE-2012-0144](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0144)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não afectado                                                                                              | Não Aplicável                                                  | (Nenhuma)                                                                                                       |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Vulnerabilidade de XSS no wizardlist.aspx                                                | [CVE-2012- 0145](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0145) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não afectado                                                                                              | Não Aplicável                                                  | (Nenhuma)                                                                                                       |  
| [MS12-012](http://go.microsoft.com/fwlink/?linkid=239941) | Vulnerabilidade de Carregamento de Biblioteca sem Segurança na Cor do Painel de Controlo | [CVE-2010-5082](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-5082)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não Aplicável                                                  | Esta vulnerabilidade foi divulgada publicamente.                                                                |  
| [MS12-013](http://go.microsoft.com/fwlink/?linkid=238617) | Vulnerabilidade de Sobrecarga de Memória Intermédia em Msvcrt.dll                        | [CVE-2012-0150](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0150)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Temporário                                                     | (Nenhuma)                                                                                                       |  
| [MS12-014](http://go.microsoft.com/fwlink/?linkid=239945) | Vulnerabilidade de Carregamento de Biblioteca sem Segurança no Codec de Áudio Indeo      | [CVE-2010-3138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3138)  | Não afectado                                                                                              | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não Aplicável                                                  | Esta vulnerabilidade foi divulgada publicamente.                                                                |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Vulnerabilidade de Corrupção de Memória no Formato de Ficheiro VSD                       | [CVE-2012-0019](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0019)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não afectado                                                                                              | Não Aplicável                                                  | Afecta o Visio Viewer 2010 e o Visio Viewer 2010 Service Pack 1 (as únicas versões suportadas do Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Vulnerabilidade de Corrupção de Memória no Formato de Ficheiro VSD                       | [CVE-2012-0020](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0020)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não afectado                                                                                              | Não Aplicável                                                  | Afecta o Visio Viewer 2010 e o Visio Viewer 2010 Service Pack 1 (as únicas versões suportadas do Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Vulnerabilidade de Corrupção de Memória no Formato de Ficheiro VSD                       | [CVE-2012-0136](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0136)  | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração          | Não afectado                                                                                              | Não Aplicável                                                  | Afecta o Visio Viewer 2010 e o Visio Viewer 2010 Service Pack 1 (as únicas versões suportadas do Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Vulnerabilidade de Corrupção de Memória no Formato de Ficheiro VSD                       | [CVE-2012-0137](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0137)  | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração          | Não afectado                                                                                              | Não Aplicável                                                  | Afecta o Visio Viewer 2010 e o Visio Viewer 2010 Service Pack 1 (as únicas versões suportadas do Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Vulnerabilidade de Corrupção de Memória no Formato de Ficheiro VSD                       | [CVE-2012-0138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0138)  | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração          | Não afectado                                                                                              | Não Aplicável                                                  | Afecta o Visio Viewer 2010 e o Visio Viewer 2010 Service Pack 1 (as únicas versões suportadas do Visio Viewer). |  
| [MS12-016](http://go.microsoft.com/fwlink/?linkid=235370) | Vulnerabilidade de Objectos Não Geridos no .NET Framework                                | [CVE-2012-0014](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0014)  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não Aplicável                                                  | (Nenhuma)                                                                                                       |  
| [MS12-016](http://go.microsoft.com/fwlink/?linkid=235370) | Vulnerabilidade de Corrupção na Área Dinâmica para Dados no .NET Framework               | [CVE-2012-0015](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0015)  | Não afectado                                                                                              | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração            | Não Aplicável                                                  | Esta vulnerabilidade foi divulgada publicamente.                                                                |
  
Localizações do Software Afectado e das Transferências  
------------------------------------------------------
  
<span></span>
As tabelas que se seguem apresentam uma lista dos boletins ordenados de acordo com as principais categorias de software e nível de gravidade.
  
**Como utilizar estas tabelas?**
  
Utilize estas tabelas para saber mais sobre as actualizações de segurança que poderá ter de instalar. Deverá rever cada programa ou componente de software listado, para confirmar se alguma das actualizações de segurança se aplica à sua instalação. Se alguma aplicação ou componente de software estiver na lista, é fornecida uma hiperligação para a actualização de software disponível e é também a apresentada a classificação da gravidade da actualização de software.
  
**Nota** Poderá ter que instalar diversas actualizações de segurança para a mesma vulnerabilidade. Reveja toda a coluna para cada identificador de boletim listado, para verificar quais as actualizações que tem que instalar, com base nos programas ou componentes que tem instalados no seu sistema.
  
#### Sistema Operativo Windows e Componentes

 
<table style="border:1px solid black;">
<tr>
<th colspan="8">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=832afe5e-d61e-4554-b889-9174df042b32)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a7d59fa8-0a49-4985-9f14-92218d3b5cea)  
(Moderada)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6025c5d6-696c-49cd-9264-96af5766d318)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5b37f5b1-207f-4fa1-9769-c873d672e80c)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=32e5c9ad-b610-4afb-b6f0-bb0b5fbdd1f6)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff2c141c-08b4-42c6-9f66-580f8678c01f)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=96d404e7-8928-494e-8a3c-3897817cda7b)  
(Moderada)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b40bc334-edbc-48d5-9196-b7fb0e19966e)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2fc9d519-94b3-4b56-92fd-4c0ccf8210fe)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=82f5c503-d2ea-4fed-8f9d-f30bee2f60b3)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f0e6e06d-89db-45ad-9660-7959c6f9b546)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c4642890-2fba-45da-bbe9-fcaa84e4aa0c)  
(Sem classificação de gravidade<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9e157b88-2c11-44dc-b13d-1051f9c39890)  
(Moderada)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bf8ad019-e710-4e16-be4f-8168df5c5343)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ee4bef7-b355-4aae-8bba-834a16d44744)  
(Importante)
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
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b81decda-9d82-4ffb-baae-78b190e553ea)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c4a52801-55b5-4eef-9db3-c29a45863198)  
(Sem classificação de gravidade<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f162ad36-c096-43ba-a440-ec4d3fb54c21)  
(Moderada)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ef4a9002-b2da-40af-abc0-737565fea179)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b53cf810-0ea3-4cb0-91f9-de1406ccfc96)  
(Importante)
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
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=8dcd71c8-82ad-4f86-b386-7f1ea09e157f)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3b42f935-7f59-4871-a01f-480033c3ad40)  
(Sem classificação de gravidade<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=24fe7c08-4736-455b-9b98-1b6a65718143)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3b18d22d-e192-498b-a105-b946a5f5bfad)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="8">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5852118c-fc39-45e2-8b44-ce1401d310e2)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6ec23c7e-0166-47dc-ae86-c49b505206bb)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bbf627df-0bc0-478f-aa34-a7e5f039e589)  
(Crítica)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d287496a-411c-4c1b-9d98-bacc553041ae)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c503c7b1-24f8-40a4-8283-c1e4abf90b57)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5161d16d-1037-49d5-8d4d-c353288cb41c)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b30a8cc5-b9ad-476f-928c-c49c993d0e80)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3a8b966a-bf34-42fd-8758-9a5e8e3c7689)  
(Crítica)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=22cc0245-1877-4c76-914f-dd68f6cd45f0)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ddbd9fcf-10c4-4089-88c0-c2a6c288222b)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73e240a6-2d5e-4ceb-8500-8dacca0e4a43)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nenhum
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=45c6c511-a4fa-4c3b-af26-6c113f6f5f5e)\*\*\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=21f7dba4-fe97-487e-8b37-45914e106db0)\*\*  
(Moderada)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=98d5b024-0eda-4e5d-ba9d-b828ad3d048e)\*\*  
(Moderada)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=025a5af0-39f1-481c-920c-43d2b3d85dc5)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c1812af-f57d-455d-a81d-5e03db99b2f7)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3f6f89b3-3bc8-4325-b8d8-9a5a398b99c6)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=046932cf-0671-49e6-8ddf-98abfc97c5f0)\*\*\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2cd8e296-dae8-41ce-8373-f8a71b4555e9)\*\*  
(Moderada)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=246f9995-fe19-43d0-8f67-0e91eb961bab)\*\*  
(Moderada)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c216e01d-2f46-4a46-bdc7-9d0fe98193a3)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1b66bb5-ea12-44a5-807a-f21ede0dc76d)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0e06e77d-7e5d-4d57-98b2-0817f68a1ebb)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=35e6bd04-594f-42ef-97f8-abcf578b4f10)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=304bd0c5-f4ee-4f8c-89b4-4cbaaf418679)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=05c0e6eb-c641-43ab-958a-f43933cdbba7)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3a96ab34-8f45-48bf-a98b-9e683b50aaa0)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=56cbeba9-0c39-4418-9042-7244ac9d03db)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d1d51b26-2d01-42a9-9bb1-9fb82c1fb914)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="8">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
Nenhum
</td>
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e5ca1bf-9415-412c-9dff-dd1abc57e74d)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8b423683-cd29-4049-82d6-f0845842e7f0)  
(Crítica)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c83a9c74-a5a7-4b3e-ba36-7a7024d99fd8)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=403f355c-2273-42ac-8263-d662f5d7740c)  
(Crítica)
</td>
<td style="border:1px solid black;">
Apenas Windows 7 para sistemas de 32 bits:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Crítica)  
Apenas Windows 7 para sistemas de 32 bits Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78cbbe02-a3d3-4cef-9b54-a3e78c1b885a)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a5d00138-4e24-4a07-92dd-3d8a14476197)  
(Crítica)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bbc9d6ae-9ec5-401f-bf16-4811b63709d1)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8bd8e804-ca4d-4326-bc60-345e2975b7aa)  
(Crítica)
</td>
<td style="border:1px solid black;">
Apenas Windows 7 para sistemas baseados em x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Crítica)  
Apenas Windows 7 para sistemas baseados em x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=299d107d-ab9f-42b6-8f94-a2f1d242c127)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6b228ad6-d5a4-4b91-8aa8-0874deb22116)\*\*\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3074a898-54bb-44ff-a8f4-77f831c28771)\*\*  
(Moderada)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=1896a6da-f7ee-484b-a97c-455fce7b82b8)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d868c5ef-165a-46a0-b832-e6ca55a910f9)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
Apenas Windows Server 2008 R2 para sistemas baseados em x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)\*  
(KB2633879)  
(Crítica)  
Apenas Windows Server 2008 R2 para sistemas baseados em x64:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)  
Apenas Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)\*  
(KB2633873)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)\*<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=576192d3-f050-4718-a7da-c84fce6bf744)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8c51e09b-51c3-4860-836e-6bcffde75f04)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=922b2438-0cfc-49e3-b9a0-52c68b69126a)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7f7c0bc3-fc26-4ee8-aedb-c251247cbeb5)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e5416371-495b-4dc7-a239-f9185f968969)  
(Crítica)
</td>
<td style="border:1px solid black;">
Apenas Windows Server 2008 R2 para sistemas baseados em Itanium:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Crítica)  
Apenas Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Crítica)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6a9b2c9-7582-4953-8ab1-a55c63fcc8dc)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fba58a1b-9d9f-4a10-b1df-08a0ebfa2358)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
</table>
 
**Notas para o Windows Server 2008 e Windows Server 2008 R2**

**\*Instalação Server Core afectada.** Esta actualização aplica-se, com a mesma classificação de gravidade, a edições suportadas do Windows Server 2008 ou Windows Server 2008 R2, conforme indicado, quer a instalação tenha sido efectuada ou não utilizando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 e Windows Server 2008 R2 como indicado, se estes tiverem sido instalados usando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*\*Instalação Server Core afectada.** Esta actualização aplica-se, com uma classificação de gravidade inferior, a edições suportadas do Windows Server 2008 ou Windows Server 2008 R2, conforme indicado, quando a instalação tenha sido efectuada utilizando a opção Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Nota para o MS12-010**

<sup>[1]</sup>As classificações de gravidade não se aplicam a esta actualização para o software especificado porque os vectores de ataque conhecidos para a vulnerabilidade conforme se discute neste boletim estão bloqueados numa configuração predefinida. No entanto, como medida de defesa profunda, a Microsoft recomenda que os clientes deste software apliquem esta actualização de segurança.

**Nota para o MS12-016**

<sup>[1]</sup>**.NET Framework 4 e .NET Framework 4 Client Profile afectados.** Os pacotes .NET Framework Redistributable versão 4 estão disponíveis em dois perfis: .NET Framework 4 e .NET Framework 4 Client Profile. O .NET Framework 4 Client Profile é um subconjunto do .NET Framework 4. A vulnerabilidade resolvida nesta actualização afecta o .NET Framework 4 e o .NET Framework 4 Client Profile. Para mais informações, consulte o artigo MSDN sobre a [Instalação do .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx).

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

#### Suites e Software do Microsoft Office

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Outro Software Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-015**](http://go.microsoft.com/fwlink/?linkid=238400)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 e Microsoft Visio Viewer 2010 Service Pack 1 (edição de 32 bits)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 e Microsoft Visio Viewer 2010 Service Pack 1 (edição de 32 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=173dc4e6-31b4-42ec-808c-f8cd005517ab)  
(KB2597170)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 e Microsoft Visio Viewer 2010 Service Pack 1 (edição de 64 bits)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 e Microsoft Visio Viewer 2010 Service Pack 1 (edição de 64 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=34b234e1-1322-4edc-829c-7bc2fbd99338)  
(KB2597170)  
(Importante)
</td>
</tr>
</table>
 

#### Software Microsoft Server

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-011**](http://go.microsoft.com/fwlink/?linkid=238500)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2010 e Microsoft Office SharePoint Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Server 2010 e Microsoft SharePoint Server 2010 Service Pack 1 (moss)](http://www.microsoft.com/downloads/details.aspx?familyid=44a8eb5a-e469-4d36-b5a0-7e030c1d3244)  
(KB2597124)  
(Importante)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft SharePoint Foundation
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-011**](http://go.microsoft.com/fwlink/?linkid=238500)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 e Microsoft SharePoint Foundation 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Foundation 2010 e Microsoft SharePoint Foundation 2010 Service Pack 1 (sts)](http://www.microsoft.com/downloads/details.aspx?familyid=dd348109-953b-4154-b265-85e4694238e6)  
(KB2553413)  
(Importante)
</td>
</tr>
</table>
 

#### Software e Ferramentas de Desenvolvimento da Microsoft

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) quando instalado em Mac  
(KB2668562)  
(Crítica)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) quando instalado em todas as edições suportadas de clientes Microsoft Windows  
(KB2668562)  
(Crítica)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) quando instalado em todas as edições suportadas de servidores Microsoft Windows  
(KB2668562)  
(Crítica)
</td>
</tr>
</table>
 
**Nota para o MS12-016**

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

Orientações e Ferramentas de Detecção e Implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para obter mais informações, visite o [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem na opção para obter as actualizações de segurança mais recentes.

As actualizações de segurança estão disponíveis no [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) e no [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). As actualizações de segurança estão também disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".

Para os clientes de Microsoft Office para Mac, o Microsoft AutoUpdate para Mac pode ajudar a manter o seu software da Microsoft actualizado. Para obter mais informações sobre como utilizar o Microsoft AutoUpdate para Mac, consulte [Verificar actualizações de software automaticamente](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Por fim, as actualizações de segurança podem ser transferidas a partir do [Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). O Catálogo do Microsoft Update permite pesquisar conteúdos disponibilizados através do Windows Update e do Microsoft Update, incluindo actualizações de segurança, controladores e service packs. Utilizando o número do boletim de segurança para pesquisar (por exemplo, "MS07-036"), pode adicionar todas as actualizações aplicáveis ao seu cesto (incluindo diferentes idiomas para uma actualização) e transferi-las para uma pasta à sua escolha. Para obter mais informação sobre o Catálogo do Microsoft Update, consulte as [Perguntas Mais Frequentes sobre o Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Orientações de detecção e implementação**

A Microsoft fornece orientações sobre detecção e implementação de actualizações de segurança. Estas orientações contêm recomendações e informação que podem auxiliar os profissionais de TI a compreender como utilizar as diversas ferramentas para detecção e implementação de actualizações de segurança. Para obter mais informações, consulte o [Artigo 961747 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/961747).

**Microsoft Baseline Security Analyzer**

O Microsoft Baseline Security Analyzer (MBSA) permite aos administradores procurar actualizações de segurança em falta e comuns erros de configuração de segurança em sistemas locais e remotos. Para obter mais informações acerca do MBSA, visite o Web site do [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Ao utilizar os Windows Server Update Services (WSUS), os administradores podem implementar de forma rápida e fiável as actualizações críticas mais recentes e as actualizações de segurança para os sistemas operativos Microsoft Windows 2000 e posteriores, Office XP e posteriores, Exchange Server 2003 e SQL Server 2000 para o Microsoft Windows 2000 e sistemas operativos posteriores.

Para obter mais informações sobre como implementar esta actualização de segurança usando os Windows Server Update Services, visite o [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

**System Center Configuration Manager 2007**

O Gestão da Actualização de Software no Configuration Manager 2007 simplifica a tarefa complexa de fornecer e gerir actualizações para sistemas de TI na empresa. Com o Configuration Manager 2007, os administradores de TI podem fornecer actualizações de produtos Microsoft a vários dispositivos, incluindo áreas de trabalho, computadores portáteis, servidores e dispositivos móveis.

A avaliação de vulnerabilidade automatizada no Configuration Manager 2007 detecta as necessidades de actualizações e comunica as acções recomendadas. A Gestão da Actualização de Software no Configuration Manager 2007 é construída a partir do Microsoft Windows Software Update Services (WSUS), uma infra-estrutura de actualização comprovada ao longo do tempo com que os administradores de TI de todo o mundo estão familiarizados. Para obter mais informações acerca de como os administradores podem utilizar o Configuration Manager 2007 para implementar actualizações, consulte [Gestão da Actualização de Software](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Para obter mais informações acerca do Configuration Manager, consulte [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx).

**Systems Management Server 2003**

O Microsoft Systems Management Server (SMS) fornece uma solução empresarial altamente configurável para gerir actualizações. O SMS permite aos administradores identificarem sistemas baseados no Windows que necessitem de actualizações de segurança e executar a implementação controlada dessas actualizações em toda a empresa, com um mínimo de incómodo para os utilizadores finais.

**Nota** O System Management Server 2003 está fora do suporte normal desde 12 de Janeiro de 2010. Para obter mais informações sobre o ciclo de vida dos produtos, visite o Web site do [Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). O próximo lançamento do SMS, System Center Configuration Manager 2007, está agora disponível; consulte a secção anterior, **System Center Configuration Manager 2007**.

Para obter mais informações acerca de como os administradores podem utilizar o SMS 2003 para implementar actualizações de segurança, consulte as informações sobre [Cenários e Procedimentos para o Microsoft Systems Management Server 2003: Distribuição de Software e Gestão de Patches](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Para obter informações sobre o SMS, consulte [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Nota** O SMS utiliza o Microsoft Baseline Security Analyzer para fornecer um suporte abrangente na detecção e implementação de actualizações dos boletins de segurança. Algumas actualizações de software poderão não ser detectadas por estas ferramentas. Nestes casos, os administradores podem utilizar as capacidades de inventário do SMS para fornecer actualizações a sistemas específicos. Para obter mais informações sobre este procedimento, consulte o artigo sobre como [Implementar actualizações de software utilizando a funcionalidade SMS Software Distribution](http://go.microsoft.com/fwlink/?linkid=33341). Algumas actualizações de segurança requerem direitos administrativos após o reinício do sistema. Os administradores podem utilizar a ferramenta Elevated Rights Deployment Tool (disponível no [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)) para instalar estas actualizações.

**Update Compatibility Evaluator e Application Compatibility Toolkit**

É frequente as actualizações utilizarem os mesmos ficheiros e configurações de registo necessários para a execução das aplicações. Isso pode dar origem a incompatibilidades e aumentar o tempo necessário para a implementação de actualizações de segurança. Pode simplificar o teste e a validação de actualizações do Windows relativamente às aplicações instaladas com os componentes do [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) incluído no [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

O Application Compatibility Toolkit (ACT) contém as ferramentas e documentação necessárias para avaliar e atenuar questões de compatibilidade da aplicação antes de implementar o Windows Vista, uma Actualização do Windows, uma Actualização de Segurança da Microsoft ou uma nova versão do Windows Internet Explorer no seu ambiente.

### Outras informações

#### Ferramenta de Remoção de Software Malicioso Windows

A Microsoft publicou uma versão actualizada da Ferramenta de Remoção de Software Malicioso para o Microsoft Windows no Windows Update, no Microsoft Update, no Windows Server Update Services e no Centro de Transferências.

#### Actualizações não relacionadas com segurança no MU, WU e WSUS

Para obter informações sobre publicações não relacionadas com segurança no Windows Update e Microsoft Update, consulte:

-   [Artigo 894199 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/894199): Descrição das alterações de conteúdo do Software Update Services e Windows Server Update Services. Inclui todos os conteúdos do Windows.
-   [Actualizações de Meses Anteriores para o Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Apresenta todas as actualizações novas, revistas e relançadas para produtos Microsoft para além do Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

Para melhorar as protecções de segurança dos clientes, a Microsoft fornece informações sobre as vulnerabilidades aos principais fornecedores de software de segurança antes de cada publicação mensal de actualizações de segurança. Os fornecedores de software de segurança podem então utilizar estas informações sobre as vulnerabilidades para assegurar protecções actualizadas aos clientes através do seu software ou dispositivos de segurança, tais como antivírus, sistemas de detecção de intrusos com base na rede ou sistemas de prevenção de intrusões com base no anfitrião. Para determinar se as protecções activas estão disponíveis nos fornecedores de software de segurança, visite os Web sites de protecções activas disponibilizados pelos parceiros do programa, indicados na lista de [parceiros do Microsoft Active Protections Program (MAPP)](http://go.microsoft.com/fwlink/?linkid=215201).

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

-   Tarjei Mandt, da [Azimuth Security](http://www.azimuthsecurity.com/), por fornecer informações sobre uma questão descrita no boletim MS12-008
-   Tarjei Mandt, da [Azimuth Security](http://www.azimuthsecurity.com/), por fornecer informações sobre duas questões descritas no boletim MS12-009
-   [Jan Schejbal](http://janschejbal.wordpress.com/), por fornecer informações sobre uma questão descrita no boletim MS12-010
-   Stephen Fewer, da [Harmony Security](http://www.harmonysecurity.com/), a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre duas questões descritas no boletim MS12-010
-   Jason Hullinger, da [HP Cloud Services](http://www.hpcloud.com/), por fornecer informações sobre uma questão descrita no boletim MS12-010
-   John Hollenberger, por fornecer informações sobre uma questão descrita no boletim MS12-011
-   Rocco Calvi, da stratsec, por fornecer informações sobre uma questão descrita no boletim MS12-011
-   Giorgio Fedon, da Minded Security, por trabalhar connosco numa actualização de protecção defensiva profunda no boletim MS12-011
-   Alexander Gavrun, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS12-013
-   Xin Ouyang, da [Palo Alto Networks](http://www.paloaltonetworks.com/), por fornecer informações sobre cinco questões descritas no boletim MS12-015
-   Jeroen Frijters, da [Sumatra](http://www.sumatra.nl/), por fornecer informações sobre uma questão descrita no boletim MS12-016

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY (1-866-727-2338). As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre as opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para obter mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (14 de Fevereiro de 2012): Publicação do Resumo dos Boletins.

*Built at 2014-04-18T01:50:00Z-07:00*
