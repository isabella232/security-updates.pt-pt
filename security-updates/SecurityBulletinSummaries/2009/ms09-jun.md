---
TOCTitle: 'MS09-JUN'
Title: Resumo dos Boletins de Segurança Microsoft de Junho 2009
ms:assetid: 'ms09-jun'
ms:contentKeyID: 61235150
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms09-jun(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Junho 2009
========================================================

Data de publicação: 9 de junho de 2009 | Updated: 10 de junho de 2009

**actualizada:** 1.1

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Junho de 2009.

Com a publicação dos boletins de Junho de 2009, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 4 de Junho de 2009. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação antecipada de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 10 de Junho de 2009, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o Webcast de boletins de segurança de Junho](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032395225). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=151361">MS09-018</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Active Directory poderiam permitir Execução Remota de Código (971055)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades comunicadas de forma privada sobre implementações do Active Directory no Microsoft Windows 2000 Server e no Windows Server 2003 e do Active Directory Application Mode (ADAM) quando instalado no Windows XP Professional e no Windows Server 2003. A mais grave das vulnerabilidades poderia permitir a execução de código remoto. Um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter o controlo total de um sistema afectado remotamente. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os procedimentos recomendados de firewall e as configurações de firewall padrão predefinidas podem ajudar a proteger as redes de ataques provenientes do exterior do perímetro da empresa. É recomendado que os sistemas ligados à Internet tenham um número mínimo de portas exposto.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141786">MS09-022</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Spooler de Impressão do Windows poderiam permitir Execução Remota de Código (961501)</strong><br />
<br />
Esta actualização de segurança resolve três vulnerabilidades no Spooler de Impressão do Windows, comunicadas de forma privada. A vulnerabilidade mais grave poderia permitir execução remota de código se um servidor afectado recebesse um pedido de RPC especialmente concebido para o efeito. Os procedimentos recomendados de firewall e as configurações de firewall padrão predefinidas podem ajudar a proteger as redes de ataques provenientes do exterior do perímetro da empresa. É recomendado que os sistemas ligados à Internet tenham um número mínimo de portas exposto.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;"><strong>Actualização de Segurança Cumulativa para o Internet Explorer (969897)</strong><br />
<br />
Esta actualização de segurança resolve sete vulnerabilidades comunicadas de forma privada e uma vulnerabilidade divulgada publicamente no Internet Explorer. A mais grave das vulnerabilidades poderia permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147416">MS09-027</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft Office Word poderiam permitir Execução Remota de Código (969514)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades comunicadas de forma privada, que poderiam permitir execução remota de código se um utilizador abrisse um ficheiro Word especialmente concebido para o efeito. Um intruso que explorasse com sucesso qualquer vulnerabilidade poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)</strong><br />
<br />
Esta actualização de segurança resolve várias vulnerabilidades comunicadas de forma privada que poderiam permitir execução remota de código se um utilizador abrisse um ficheiro Excel especialmente concebido para o efeito que incluísse um registo de objecto mal formado. Um intruso que conseguisse tirar partido de qualquer uma destas vulnerabilidades poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=128104">MS09-024</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade em Conversores do Microsoft Works poderia permitir Execução Remota de Código (957632)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada em conversores do Microsoft Works. Esta vulnerabilidade poderia permitir a execução remota de código se um utilizador abrisse um ficheiro Works especialmente concebido para o efeito. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150174">MS09-026</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na RPC poderia permitir Elevação de Privilégios (970238)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente sobre a funcionalidade de chamada de procedimento remoto (RPC) do Windows em que o Motor de Marshalling da RPC não actualiza adequadamente o seu estado interno. A vulnerabilidade poderia permitir que um intruso executasse código arbitrário e assumisse o controlo total de um sistema afectado. As edições suportadas do Microsoft Windows não são fornecidas com quaisquer servidores ou clientes de RPC que estejam sujeitos à exploração desta vulnerabilidade. Numa configuração predefinida, os utilizadores não poderiam ser atacados pela exploração desta vulnerabilidade. No entanto, a vulnerabilidade está presente no runtime da RPC do Microsoft Windows e poderia afectar aplicações de RPC de terceiros.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Kernel do Windows poderiam permitir Elevação de Privilégios (968537)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades divulgadas publicamente e duas comunicadas de forma privada sobre o kernel do Windows que poderiam permitir elevação de privilégios. Um intruso que conseguisse explora qualquer uma destas vulnerabilidades com sucesso poderia executar código arbitrário e obter controlo total de um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Um intruso teria que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar estas vulnerabilidades. As vulnerabilidades não poderiam ser exploradas remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150568">MS09-020</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Internet Information Services (IIS) poderiam permitir Elevação de Privilégios (970483)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente e uma vulnerabilidade comunicada de forma privada no Microsoft Internet Information Services (IIS). As vulnerabilidades poderiam permitir elevação de privilégios se um intruso enviasse um pedido HTTP especialmente concebido para o efeito para um Web site que exigisse autenticação. Estas vulnerabilidades permitem que um intruso ignore a configuração do IIS que especifica que tipo de autenticação é permitido, mas não a verificação da lista de controlo de acesso (ACL) baseada no sistema de ficheiros que verifica se um determinado utilizador tem direitos de acesso a um ficheiro. Uma exploração destas vulnerabilidades com sucesso continuaria a restringir o intruso às permissões concedidas à conta de utilizador anónimo pelas ACLs do sistema de ficheiros.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=143550">MS09-023</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Windows Search poderia permitir a Divulgação de Informações (963093)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Windows Search, comunicada de forma privada. A vulnerabilidade poderia permitir a divulgação de informações se um utilizador executasse uma pesquisa cujo primeiro resultado fosse um ficheiro especialmente concebido para o efeito ou se o utilizador pré-visualizasse um ficheiro especialmente concebido para o efeito a partir dos resultados da pesquisa. Por predefinição, o componente do Windows Search não é pré-instalado no Microsoft Windows XP e Windows Server 2003. É um componente opcional disponível para transferência. O Windows Search instalado em edições suportadas do Windows Vista e Windows Server 2008 não é afectado por esta vulnerabilidade.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Moderada</a><br />
Divulgação de Informações</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Índice de possibilidade de exploração  
-------------------------------------
  
<span></span>
A tabela que se segue fornece uma avaliação da possibilidade de exploração para cada uma das vulnerabilidades abordadas este mês. As vulnerabilidades encontram-se listadas por ordem de identificação do boletim e de CVE.
  
**Como utilizar esta tabela?**
  
Utilize esta tabela para saber mais sobre a probabilidade de códigos de exploração funcionais serem lançados no espaço de 30 dias após o lançamento do boletim de segurança, para cada uma das actualizações de segurança que poderá ter de instalar. Deverá rever cada avaliação em baixo, conforme a sua configuração específica, para dar prioridade à sua implementação. Para obter mais informações sobre o significado destas classificações e sobre como elas são estabelecidas, consulte o [Índice de Possibilidade de Exploração da Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identificação do Boletim                                  | Título do Boletim                                                                                          | ID de CVE                                                                        | Avaliação do índice de possibilidade de exploração                                                               | Notas principais                                                                                                                                                                                                                                                                                                   |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-018](http://go.microsoft.com/fwlink/?linkid=151361) | Vulnerabilidades no Active Directory poderiam permitir Execução Remota de Código (971055)                  | [CVE-2009-1138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1138) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Existe uma possibilidade de execução remota de código em servidores Windows 2000 que expõem o serviço LDAP (default tcp/389) na rede.                                                                                                                                                                              |  
| [MS09-018](http://go.microsoft.com/fwlink/?linkid=151361) | Vulnerabilidades no Active Directory poderiam permitir Execução Remota de Código (971055)                  | [CVE-2009-1139](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1139) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | O efeito de segurança desta vulnerabilidade consiste numa fuga de memória que poderá acabar por conduzir à negação de serviço. A execução de código não é possível.                                                                                                                                                |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2007-3091](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2007-3091) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2009-1140](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1140) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Esta é uma vulnerabilidade de acesso a informações entre domínios que resulta, muito provavelmente, em divulgação de informações e não em execução de código.                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2009-1141](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1141) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2009-1528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1528) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2009-1529](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1529) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2009-1530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1530) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2009-1531](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1531) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Actualização de Segurança Cumulativa para o Internet Explorer (969897)                                     | [CVE-2009-1532](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1532) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-020](http://go.microsoft.com/fwlink/?linkid=150568) | Vulnerabilidades no Internet Information Services (IIS) poderiam permitir Elevação de Privilégios (970483) | [CVE-2009-1122](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1122) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Probabilidade baixa de execução de código mas probabilidade elevada de divulgação de informações devido a condições que ignoram a autenticação.                                                                                                                                                                    |  
| [MS09-020](http://go.microsoft.com/fwlink/?linkid=150568) | Vulnerabilidades no Internet Information Services (IIS) poderiam permitir Elevação de Privilégios (970483) | [CVE-2009-1535](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1535) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | O código público está disponível para divulgação de informações.                                                                                                                                                                                                                                                   |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)            | [CVE-2009-0549](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0549) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)            | [CVE-2009-0557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0557) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)            | [CVE-2009-0558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0558) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)            | [CVE-2009-0559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0559) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | Existe uma ameaça de execução de código apenas para o Office 2000. É improvável que ataques a versões posteriores do Office resultem em execução de código.                                                                                                                                                        |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)            | [CVE-2009-0560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0560) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)            | [CVE-2009-0561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0561) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Vulnerabilidades no Microsoft Office Excel poderiam permitir Execução Remota de Código (969462)            | [CVE-2009-1134](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1134) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Vulnerabilidades no Spooler de Impressão do Windows poderiam permitir Execução Remota de Código (961501)   | [CVE-2009-0228](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0228) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Vulnerabilidades no Spooler de Impressão do Windows poderiam permitir Execução Remota de Código (961501)   | [CVE-2009-0229](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0229) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Trata-se de uma vulnerabilidade de divulgação de informações sem possibilidade de execução de código.                                                                                                                                                                                                              |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Vulnerabilidades no Spooler de Impressão do Windows poderiam permitir Execução Remota de Código (961501)   | [CVE-2009-0230](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0230) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-023](http://go.microsoft.com/fwlink/?linkid=143550) | Vulnerabilidade no Windows Search poderia permitir a Divulgação de Informações (963093)                    | [CVE-2009-0239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0239) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-024](http://go.microsoft.com/fwlink/?linkid=128104) | Vulnerabilidade em Conversores do Microsoft Works poderia permitir Execução Remota de Código (957632)      | [CVE-2009-1533](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1533) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Vulnerabilidades no Kernel do Windows poderiam permitir Elevação de Privilégios (968537)                   | [CVE-2009-1123](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1123) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Vulnerabilidades no Kernel do Windows poderiam permitir Elevação de Privilégios (968537)                   | [CVE-2009-1124](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1124) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Vulnerabilidades no Kernel do Windows poderiam permitir Elevação de Privilégios (968537)                   | [CVE-2009-1125](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1125) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Vulnerabilidades no Kernel do Windows poderiam permitir Elevação de Privilégios (968537)                   | [CVE-2009-1126](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1126) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | O código de exploração consistente é mais provável no Windows 2000. A probabilidade de execução de código a partir desta vulnerabilidade de sobrecarga da memória intermédia da pilha é reduzida no Windows XP e Windows Server 2003 devido à protecção /GS.                                                       |  
| [MS09-026](http://go.microsoft.com/fwlink/?linkid=150174) | Vulnerabilidade na RPC poderia permitir Elevação de Privilégios (970238)                                   | [CVE-2009-0568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0568) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | Esta vulnerabilidade não afecta directamente qualquer software Microsoft. No entanto, as estações de trabalhos onde os serviços RPC são implementados por fornecedores de software independentes poderão estar susceptíveis à execução remota de código, caso esta actualização de segurança não esteja instalada. |  
| [MS09-027](http://go.microsoft.com/fwlink/?linkid=147416) | Vulnerabilidades no Microsoft Office Word poderiam permitir Execução Remota de Código (969514)             | [CVE-2009-0563](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0563) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                                                                                                                                                                          |  
| [MS09-027](http://go.microsoft.com/fwlink/?linkid=147416) | Vulnerabilidades no Microsoft Office Word poderiam permitir Execução Remota de Código (969514)             | [CVE-2009-0565](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0565) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                                                                                                                                                                          |
  
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
</tr>
<tr>
<th colspan="8">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Active Directory no Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bba6e20a-0345-46ae-a6f1-fd27fdee7c21)  
(KB969805)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=86378753-db24-44c2-a27d-cc0239f40ab8)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d645ad82-13c3-4030-808b-834e86ed3298)  
(Crítica)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fe8b3796-a407-4f41-89eb-35b4bcc24ff6)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=155a79c1-e5e4-4f62-b4b0-53aca59f20ac)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=79b0481d-a3d7-477b-928a-a98cc79374af)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=8515a294-4f25-4dc5-860a-e7ad9b6c1c01)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="8">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 e Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM) no Windows XP Professional Service Pack 2 e Windows XP Professional Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cb2c9b76-0c65-4754-9941-d45a7c74a29a)  
(KB970437)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f2119aca-a98e-4810-be52-f38241443baf)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3d7f63ee-d7c3-48a5-902e-60625405e97d)  
(Crítica)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=827b735c-660b-4723-b688-3297e107153a)  
(Crítica)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d9e27ce1-4e7c-437f-9477-e7805a33da08)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f033fa78-c451-44f8-aa6c-a49622c37f40)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6349e046-a3f8-4ae5-b8c3-c9879cc99e8f)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 5.1 no Windows XP Professional Service Pack 2 e Windows XP Professional Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=97da589f-4534-42f6-9f29-967b5a33c542)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=759f22cb-ea7f-49dd-a200-19cb83fffd8d)  
(Moderada)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=2ef3aaf0-a2a9-4c17-99ab-a0dc3d3f7e86)  
(KB970437)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22699d09-1e68-456a-8733-bfad6667ebf5)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=088f70eb-c5c5-426a-880a-18ed386d0b56)  
(Crítica)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e5d2c81e-ffab-4e3b-a59a-a55000597213)  
(Crítica)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a24aedf0-7a31-4ee8-a9a6-998f1160c700)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=20734b70-37f1-47dd-bc09-d56f93577a55)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3769800e-af93-4a44-8a1e-b30cc54b226f)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=8982e6d2-e1f7-4208-88e3-80b159a8e21a)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=50c56dd6-c34d-4632-a779-8bcf8fdb341b)  
(Moderada)
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=d814ce65-a193-4027-a6cd-106d388830a6)   
(KB969805)  
(Importante)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=f6f99957-f74f-4446-8734-a468283eebae)   
(KB970437)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=865414f8-3f77-4fee-acc6-6684a3dc0aa4)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=72a23752-86fb-4cc9-ab8e-63ffdfae5bec)  
(Moderada)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a980b867-c67f-4c61-b6db-e55c2ca68dc0)  
(Moderada)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=298143f2-f37a-4a2c-86ac-9804d4ff1dad)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62bb9e22-4f4b-4ffc-ba76-f626e94c79d5)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9356404c-d89a-4de0-b9b4-f6e1bdadf745)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=2bd4e410-dbd8-431a-b316-e1e2f1825c3a)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=e72ef31f-5161-4fe6-8ed3-6206e02cef31)  
(Moderada)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=0d1f23c8-06eb-4996-92eb-0eb635fd6a42)  
(KB969805)  
(Importante)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=1a2badc7-c0a5-4032-a009-73ebe9d76313)  
(KB970437)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=197a6cc7-4ba3-4d2e-b621-0ef3da645ef2)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2a03d3c4-e39d-43a3-8d42-216e9551be96)  
(Moderada)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5e7d6372-9c8c-449d-88fd-afd4f92ad9e6)  
(Moderada)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4a5401d7-ca97-4734-a0e9-d7ffe0777e34)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=888b8dd8-d76c-42f5-a377-1f1750d3cf56)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5a3123af-173d-49eb-9997-14e82e764aee)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=ea363223-535d-4142-9aba-3890960c6259)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=7ffc3680-f9bf-423b-96a7-102f4cc9c240)  
(Moderada)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=92e7808b-92ff-449d-bb73-ee8638e9ccd1)  
(KB969805)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=719efd62-fb33-447d-b6dd-2aaafbbad881)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=58efde2c-e0b8-4259-b19e-80564b834882)  
(Moderada)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a2d2907e-67ae-44a4-a805-8670e659ea57)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3084f46e-02b9-4d99-a7a1-033817f9bd9f)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=13b50993-410f-4e7a-a33a-6d9b48dbb4d1)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=e6b806eb-e2c4-4436-8964-720db593055d)  
(Importante)
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
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3ad8f037-2434-4dea-bfc3-9d3b4008b828)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e60215c3-b8b9-4e45-9d9f-b3fb0b47cce1)  
(Crítica)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6f2730e9-b4fc-4f20-96cf-73f1be63f374)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ca227c0-f2dd-429c-a542-e08e93527214)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c31b36f8-330c-4a0c-9a3d-7cbe9a1ab8c8)  
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
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85c317cd-2a14-4747-9f50-3af3ddd3ae1b)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=88185088-8c2c-4bc6-89b2-87f4d4849cf7)  
(Crítica)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5edb14f7-11ec-4180-9f0f-b2673f1c8d83)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=188adafe-1feb-46ad-b237-a88d35104dcd)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d70a65f-07ce-4992-8bec-28fefd7587bc)  
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
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
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
Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f18356d-9f09-4d24-8361-970c0d1ccac4)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a0e3f975-57da-43fa-ac12-3d14fd6ce939)\*\*  
(Moderada)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=aaad301c-d232-4733-a0df-8e5d41bbfde8)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaa26c6c-5bf7-4099-bb21-1e03de3a25ca)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98ba52b2-da1a-4939-a10e-d43b3a7e7ed4)\*  
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
Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d0a6e8d-a31d-4f3d-a7d7-e61215bfebed)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=758edce7-2a82-4b2e-bd71-5b7075cc4b17)\*\*  
(Moderada)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=faac92d4-4a2b-4bb5-8bd1-1519a9fa8147)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=447aaa4f-946b-4f23-b151-dcf46ea9f80e)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbaa5a72-c267-4907-a207-525c2803d7b9)\*  
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
Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bbac3deb-6c93-45aa-832c-02b915ac7f44)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=67d4c189-030d-42eb-98b9-7957ccd92592)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f33012b9-5d5b-4f72-8d49-a8e1c8bc1337)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0e3ad56-a363-44ba-af4d-b7f551c88afd)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
</table>
 
**Notas para o Windows Server 2008**

**\*Instalação Server Core do Windows Server 2008 afectada.** Para edições suportadas do Windows Server 2008, esta actualização aplica-se com a mesma classificação de gravidade, quer o Windows Server 2008 tenha ou não sido instalado utilizando a opção de instalação Server Core. Para mais informações sobre esta opção de instalação, consulte a informação sobre [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core do Windows Server 2008 não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 se este tiver sido instalado usando a opção de instalação Server Core. Para mais informações sobre esta opção de instalação, consulte a informação sobre [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Suites e Software do Microsoft Office

 
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
</tr>
<tr>
<th colspan="4">
Suites, Sistemas e Componentes do Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3663e9f2-a952-4238-b902-90b5b09feb38)  
(KB969600)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd16e243-b8e2-4afb-86b6-4d60214598eb)  
(KB969683)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4bf95806-3d32-411b-9779-a81aebad45e9)  
(KB957838)  
(Crítica)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1323be1-15f2-491b-abae-c03ba1394398)  
(KB969602)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd80ce95-0aec-4493-b9d1-c3dad95c3415)  
(KB969680)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b0ba8c9e-75ee-46bd-9e92-d4e6599309ad)  
(KB957646)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7cbc2587-2c8c-49b4-9f40-e4cdccb61ecd)  
(KB969603)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=10156044-a5a4-4312-98a7-1b1ced625ddb)  
(KB969681)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3 com o Conversor de Ficheiros do Microsoft Works 6–9](http://www.microsoft.com/downloads/details.aspx?familyid=a7ba3ea7-d06a-4c14-9107-9b92ef68fcae)\*\*\*  
(KB968326)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 1 e Microsoft Office System 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1 e Microsoft Office Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7e205108-4c28-4cab-a4d0-4ed3fd696473)  
(KB969604)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1 e Microsoft Office Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2bcd565a-6acb-407d-80da-0398526ddf99)\*  
(KB969682)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bd47e1e5-cd2e-4c08-9864-471e97f38ca3)  
(KB969559)  
(Importante)
</td>
</tr>
<tr>
<th colspan="4">
Microsoft Office para Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
<td style="border:1px solid black;">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 para Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 para Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Conversor de Formato de Ficheiros Open XML para Mac
</td>
<td style="border:1px solid black;">
[Conversor de Formato de Ficheiros Open XML para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Importante)
</td>
<td style="border:1px solid black;">
[Conversor de Formato de Ficheiros Open XML para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="4">
Outro Software Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=20e6933d-85f8-4cec-9534-893789cd053e)  
(KB969685)  
(Importante)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=ac0530dc-7f63-4ad0-85c1-784ad28156cf)  
(KB969686)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
(Importante)  
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
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
Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 1 e Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63bd8f14-e736-46ce-af66-d30f17461e5a)  
(KB969613)  
(Importante)
</td>
<td style="border:1px solid black;">
[Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 1 e Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2)  
(KB969679)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=628280fe-e035-4274-85f2-393d9bad543c)  
(KB967043)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=f6fa110e-45c6-450f-ae47-c89a06e3f762)  
(KB967044)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 1 e Microsoft Office SharePoint Server 2007 Service Pack 2 (edições de 32 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=862e6ad1-8124-4060-93b1-2b882ef5ce3d)\*\*  
(KB969737)  
(Importante)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 e Microsoft Office SharePoint Server 2007 Service Pack 2 (edições de 64 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=b7b6e611-2c5d-4639-add9-972055789ecd)\*\*  
(KB969737)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
</table>
 
**Notas para o boletim MS09-021**

\*Para o Microsoft Office Excel 2007 Service Pack 1 e o Microsoft Office Excel 2007 Service Pack 2, para além do pacote de actualização de segurança KB969682, os clientes têm também de instalar a actualização de segurança para o [Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 1 e o Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2) (KB969679) para estarem protegidos contra as vulnerabilidades descritas neste boletim.

\*\*Esta actualização aplica-se a servidores com o Excel Services instalado, como a configuração predefinida do Microsoft Office SharePoint Server 2007 Enterprise e Microsoft Office SharePoint Server 2007 For Internet Sites. O Microsoft Office SharePoint Server 2007 Standard não inclui o Excel Services.

**Nota para o boletim MS09-024**

\*\*\*O Microsoft Office Word 2003 é afectado se for instalado um conversor do Works vulnerável. Os conversores do Works estão disponíveis para o Microsoft Office Word 2003 como transferência a partir do [Conversor de Ficheiros do Microsoft Works 6–9](http://www.microsoft.com/downloads/details.aspx?familyid=bf41401e-70fa-465d-ae2e-cf44dbf05297&displaylang=en).

Orientações e ferramentas de detecção e implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para mais informações, visite o [Centro de Gestão de Actualizações TechNet](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em Casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem na opção para obter as actualizações de segurança mais recentes.

As actualizações de segurança estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt), no [Windows Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt) e no [Office Update](http://office.microsoft.com/pt-pt/downloads/default.aspx). As actualizações de segurança estão também disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".

Finalmente, as actualizações de segurança podem ser transferidas a partir do [Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). O Catálogo do Microsoft Update permite pesquisar conteúdos disponibilizados através do Windows Update e do Microsoft Update, incluindo actualizações de segurança, controladores e service packs. Utilizando o número do boletim de segurança para pesquisar (por exemplo, "MS07-036"), pode adicionar todas as actualizações aplicáveis ao seu cesto (incluindo diferentes idiomas para uma actualização) e transferi-las para uma pasta à sua escolha. Para mais informação sobre o Catálogo do Microsoft Update, consulte as [Perguntas Mais Frequentes sobre o Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Orientações de detecção e implementação**

A Microsoft forneceu orientações sobre a detecção e implementação das actualizações de segurança deste mês. Estas orientações também auxiliarão os profissionais de informática a compreenderem de que forma podem usar diferentes ferramentas de suporte à implementação de actualizações de segurança, tais como o Windows Update, o Microsoft Update, o Office Update, o Microsoft Baseline Security Analyzer (MBSA), a Office Detection Tool, o Microsoft Systems Management Server (SMS) e a Extended Security Update Inventory Tool (ESUIT). Para obter mais informações, consulte o [Artigo 910723 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

O Microsoft Baseline Security Analyzer (MBSA) permite aos administradores procurar actualizações de segurança em falta e comuns erros de configuração de segurança em sistemas locais e remotos. Para obter mais informações acerca do MBSA, visite o Web site do [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Ao utilizar os Windows Server Update Services (WSUS), os administradores podem rápida e fiavelmente implementar as actualizações críticas mais recentes e as actualizações de segurança para os sistemas operativos Windows 2000 e posteriores, Office XP e posteriores, Exchange Server 2003 e SQL Server 2000 para Windows 2000 e sistemas operativos posteriores.

Para mais informações sobre como implementar esta actualização de segurança usando os Windows Server Update Services, visite o [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

O Microsoft Systems Management Server (SMS) fornece uma solução empresarial altamente configurável para gerir actualizações. O SMS permite aos administradores identificarem sistemas baseados no Windows que necessitem de actualizações de segurança e executar a implementação controlada dessas actualizações em toda a empresa, com um mínimo de incómodo para os utilizadores finais. O próximo lançamento do SMS, System Center Configuration Manager 2007, está agora disponível; consulte também [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Para mais informações sobre como os administradores podem utilizar o SMS 2003 para implementar actualizações de segurança, consulte [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Os utilizadores do SMS 2.0 também podem utilizar o [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) para ajudar na implementação das actualizações de segurança. Para informações sobre o SMS, visite [Microsoft Systems Management Server](http://www.microsoft.com/portugal/smserver/default.mspx).

**Nota** O SMS utiliza as ferramentas Microsoft Baseline Security Analyzer e Microsoft Office Detection Tool para fornecer um suporte abrangente na detecção e implementação de actualizações dos boletins de segurança. Algumas actualizações de software poderão não ser detectadas por estas ferramentas. Nestes casos, os administradores podem utilizar as capacidades de inventário do SMS para fornecer actualizações a sistemas específicos. Para mais informações sobre este procedimento, veja o artigo sobre como [Implementar actualizações de software utilizando a funcionalidade SMS Software Distribution](http://go.microsoft.com/fwlink/?linkid=33341). Algumas actualizações de segurança requerem direitos administrativos após o reinício do sistema. Os administradores podem utilizar a ferramenta Elevated Rights Deployment Tool (disponível no [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) e no [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)) para instalar estas actualizações.

**Update Compatibility Evaluator e Application Compatibility Toolkit**

É frequente as actualizações utilizarem os mesmos ficheiros e configurações de registo necessários para a execução das aplicações. Isso pode dar origem a incompatibilidades e aumentar o tempo necessário para a implementação de actualizações de segurança. Pode simplificar o teste e a validação de actualizações do Windows relativamente às aplicações instaladas com os componentes do [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) incluído no [Application Compatibility Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

O Application Compatibility Toolkit (ACT) contém as ferramentas e documentação necessárias para avaliar e atenuar questões de compatibilidade da aplicação antes de implementar o Microsoft Windows Vista, uma Actualização do Windows, uma Actualização de Segurança da Microsoft ou uma nova versão do Windows Internet Explorer no seu ambiente.

### Outras informações

#### Ferramenta de Remoção de Software Malicioso Windows

A Microsoft publicou uma versão actualizada da Ferramenta de Remoção de Software Malicioso para o Microsoft Windows no Windows Update, no Microsoft Update, no Windows Server Update Services e no Centro de Transferências.

#### Actualizações não relacionadas com segurança, de elevada prioridade, no MU, WU e WSUS

Para obter informações sobre publicações não relacionadas com segurança no Windows Update e Microsoft Update, consulte:

-   [Artigo 894199 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/894199): Descrição das alterações de conteúdo do Software Update Services e Windows Server Update Services. Inclui todos os conteúdos do Windows.
-   [Actualizações Novas, Revistas e Publicadas para Produtos Microsoft que não Microsoft Windows](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

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

-   Joshua J. Drake, da [VeriSign iDefense Labs](http://labs.idefense.com/), por fornecer informações sobre uma questão descrita no boletim MS09-018
-   Justin Wyatt, da [Beaverton School District](http://www.beaverton.k12.or.us/home/), por fornecer informações sobre uma questão descrita no boletim MS09-018
-   David Bloom, da [Google Inc.](http://www.google.com/), por trabalhar connosco numa questão descrita no boletim MS09-019
-   Jorge Luis Alvarez Medina, da [Core Security Technologies](http://www.coresecurity.com/), por fornecer informações sobre uma questão descrita no boletim MS09-019
-   Haifei Li, da [Fortinet](http://www.fortinet.com/), por fornecer informações sobre uma questão descrita no boletim MS09-019
-   [Tippingpoint](http://www.tippingpoint.com/) e [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecerem informações sobre uma questão descrita no boletim MS09-019
-   Peter Vreugdenhil, a trabalhar com a [Tippingpoint](http://www.tippingpoint.com/) e a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecer informações sobre uma questão descrita no boletim MS09-019
-   Wushi, a trabalhar com a [Tippingpoint](http://www.tippingpoint.com/) e a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecer informações sobre duas questões descritas no boletim MS09-019
-   Nils, a trabalhar com a [Tippingpoint](http://www.tippingpoint.com/) e a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecer informações sobre uma questão descrita no boletim MS09-019
-   Yamata Li, da [Palo Alto Networks](http://www.paloaltonetworks.com/), por fornecer informações sobre uma questão descrita no boletim MS09-020
-   Bing Liu, da [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) da Fortinet, por fornecer informações sobre três questões descritas no boletim MS09-021
-   Carsten H. Eiram, da [Secunia](http://secunia.com/), por fornecer informações sobre duas questões descritas no boletim MS09-021
-   [Equipa de investigação de vulnerabilidades da TELUS Security Labs](http://telussecuritylabs.com/), por fornecer informações sobre uma questão descrita no boletim MS09-021
-   Sean Larsson e Joshua Drake, da [VeriSign iDefense Labs](http://labs.idefense.com/), por fornecerem informações sobre uma questão descrita no boletim MS09-021
-   [TippingPoint](http://www.tippingpoint.com/) e [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecerem informações sobre uma questão descrita no boletim MS09-021
-   Jun Mao, da [iVeriSign iDefense Labs](http://labs.idefense.com/), por fornecer informações sobre uma questão descrita no boletim MS09-022
-   Yair Amit, da [IBM Rational Application Security](http://blog.watchfire.com/), por fornecer informações sobre uma questão descrita no boletim MS09-023
-   Shaun Colley, da [NGS Software](http://www.ngssoftware.com/), por fornecer informações sobre uma questão descrita no boletim MS09-024
-   Thomas Garnier, por fornecer informações sobre duas questões descritas no boletim MS09-025
-   Wushi, da [team509](http://www.team509.com/), a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecer informações sobre uma questão descrita no boletim MS09-027
-   Nicolas Joly, da [VUPEN Security](http://www.vupen.com/), por fornecer informações sobre uma questão descrita no boletim MS09-027

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (9 de Junho de 2009): Publicação do Resumo dos Boletins.
-   V1.1 (10 de Junho de 2009): Correcção do rating e key notes para o CVE-2009-1138 no indice de possibilidade de Exploração.

*Built at 2014-04-18T01:50:00Z-07:00*
