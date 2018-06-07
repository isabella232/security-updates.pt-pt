---
TOCTitle: 'MS10-AUG'
Title: Resumo dos Boletins de Segurança Microsoft de Agosto 2010
ms:assetid: 'ms10-aug'
ms:contentKeyID: 61235154
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms10-aug(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Agosto 2010
=========================================================

Data de publicação: 2 de agosto de 2010 | Updated: 1 de setembro de 2010

**actualizada:** 2.1

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Agosto de 2010.

Com a publicação dos boletins de Agosto de 2010, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 5 de Agosto de 2010. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 11 de Agosto de 2010, às 11:00, hora do Pacífico (Estados Unidos e Canadá). Registe-se agora para o [Webcast de Boletins de Segurança de Agosto](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454431&eventcategory=4&culture=en-us&countrycode=us). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

No que se refere ao boletim de segurança fora do ciclo regular [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393), anunciado originalmente na versão 1.0 deste resumo dos boletins, a Microsoft publicou a notificação antecipada de boletins correspondente a 30 de Julho de 2010 e fez um webcast de boletins a 2 de Agosto de 2010. Este webcast de [2 de Agosto de 2010](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032456779&culture=en-us) está disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197393">MS10-046</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na Shell do Windows Poderia Permitir Execução Remota de Código (2286198)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade na Shell do Windows divulgada publicamente. A vulnerabilidade poderia permitir a execução remota de código se o ícone de um atalho especialmente concebido para o efeito fosse apresentado. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197104">MS10-049</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no SChannel Poderiam Permitir Execução Remota de Código (980436)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente e uma vulnerabilidade comunicada de forma privada no pacote de segurança Secure Channel (SChannel) do Windows. A vulnerabilidade mais grave poderia permitir a execução remota de código se um utilizador visitasse um Web site especialmente concebido para o efeito que fosse concebido para explorar estas vulnerabilidades através de um browser da Web na Internet. Contudo, em qualquer dos casos, o intruso não teria forma de forçar os utilizadores a visitar estes Web sites. Em vez disso, o intruso teria de persuadir os utilizadores a visitar o Web site, levando-os normalmente a clicar numa hiperligação numa mensagem de correio electrónico, ou num pedido de mensagem instantânea que leva o utilizador para o Web site do intruso.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196268">MS10-051</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft XML Core Services Poderia Permitir Execução Remota de Código (2079403)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft XML Core Services comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer. Um intruso não teria como obrigar os utilizadores a visitar estes Web sites. Em vez disso, um intruso teria de persuadir os utilizadores a visitar o Web site, levando-os normalmente a clicar numa hiperligação presente numa mensagem de correio electrónico, ou num programa de mensagens instantâneas, que levasse o utilizador para o Web site do intruso.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194432">MS10-052</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade em Codecs Microsoft MPEG Layer-3 Poderia Permitir Execução Remota de Código (2115168)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada nos codecs de áudio Microsoft MPEG Layer-3. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro multimédia ou se recebesse conteúdo de transmissão em sequência especialmente concebidos para o efeito a partir de um Web site ou de qualquer aplicação que entregue conteúdos Web. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196549">MS10-053</a></td>
<td style="border:1px solid black;"><strong>Actualização de Segurança Cumulativa para o Internet Explorer (2183461)</strong><br />
<br />
Esta actualização de segurança resolve seis vulnerabilidades no Internet Explorer, comunicadas de forma privada. As vulnerabilidades mais graves poderiam permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190318">MS10-054</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Servidor SMB Poderiam Permitir Execução Remota de Código (982214)</strong><br />
<br />
Esta actualização de segurança resolve várias vulnerabilidades no Microsoft Windows, comunicadas de forma privada. A mais grave destas vulnerabilidades poderia permitir a execução remota de código, se um intruso criasse um pacote SMB especialmente concebido para o efeito e o enviasse a um sistema afectado. Os procedimentos recomendados em relação à utilização de firewalls e as predefinições padrão de uma firewall podem ajudar a proteger as redes de ataques provenientes do exterior do perímetro da empresa que poderiam tentar explorar estas vulnerabilidades.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194906">MS10-055</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Codec Cinepak Poderia Permitir Execução Remota de Código (982665)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Codec Cinepack comunicada de forma privada. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro multimédia ou se recebesse conteúdo de transmissão em sequência especialmente concebidos para o efeito a partir de um Web site ou de qualquer aplicação que entregue conteúdos Web. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196938">MS10-056</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Microsoft Office Word Poderiam Permitir Execução Remota de Código (2269638)</strong><br />
<br />
Esta actualização de segurança resolve quatro vulnerabilidades no Microsoft Office, comunicadas de forma privada. As vulnerabilidades mais graves poderiam permitir a execução remota de código se um utilizador abrisse ou pré-visualizasse uma mensagem de correio electrónico maliciosa em formato RTF especialmente concebida para o efeito. Um intruso que conseguisse explorar qualquer uma destas vulnerabilidades com sucesso poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179830">MS10-060</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Common Language Runtime do Microsoft. NET e no Microsoft Silverlight Poderiam Permitir Execução Remota de Código (2265906)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades no Microsoft. NET Framework e Microsoft Silverlight, comunicadas de forma privada. As vulnerabilidades poderiam permitir a execução remota de código num sistema cliente se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando um browser da Web que pudesse executar Aplicações de Browser XAML (XBAPs) ou aplicações Silverlight, ou se um intruso tivesse sucesso em convencer um utilizador a executar uma aplicação do Microsoft. NET especialmente concebida para o efeito. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. As vulnerabilidades também poderiam permitir a execução remota de código num sistema de servidor a executar o IIS, se esse servidor permitisse o processamento de páginas ASP.NET e se um intruso tivesse sucesso em actualizar uma página ASP.NET especialmente concebida para o efeito para esse servidor e executá-la, como poderia ser o caso de um cenário de alojamento Web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework, Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=195812">MS10-047</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Kernel do Windows Poderiam Permitir Elevação de Privilégios (981852)</strong><br />
<br />
Esta actualização de segurança resolve várias vulnerabilidades no Microsoft Windows, comunicadas de forma privada. A mais grave destas vulnerabilidades poderia permitir elevação de privilégios se um intruso iniciasse sessão localmente e executasse uma aplicação especialmente concebida para o efeito. Um intruso teria que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar estas vulnerabilidades. As vulnerabilidades não poderiam ser exploradas remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194552">MS10-048</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades nos Controladores de Modo de Kernel do Windows Poderiam Permitir Elevação de Privilégios (2160329)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente e quatro vulnerabilidades comunicadas de forma privada nos controladores de modo de kernel do Windows. A vulnerabilidade mais grave poderia permitir elevação de privilégios se um intruso iniciasse sessão num sistema afectado e executasse uma aplicação especialmente concebida para o efeito. Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar esta vulnerabilidade. A vulnerabilidade não poderia ser explorada remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197103">MS10-050</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Windows Movie Maker Poderia Permitir Execução Remota de Código (981997)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Windows Movie Maker comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um intruso enviasse um ficheiro de projecto do Movie Maker especialmente concebido para o efeito e convencesse o utilizador a abrir o ficheiro especialmente concebido para o efeito. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196275">MS10-057</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft Office Excel Poderia Permitir Execução Remota de Código (2269707)</strong> <br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Office, comunicada de forma privada. Esta vulnerabilidade poderia permitir a execução remota de código se um utilizador abrisse um ficheiro Excel especialmente concebido para o efeito. Um intruso que conseguisse explorar esta vulnerabilidade com êxito poderia obter os mesmos privilégios que o utilizador com sessão iniciada. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194562">MS10-058</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no TCP/IP Poderiam Permitir Elevação de Privilégios (978886)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades no Microsoft Windows, comunicadas de forma privada. A mais grave destas vulnerabilidades poderia permitir elevação de privilégios devido a um erro no processamento de uma memória intermédia de entrada específica. Um intruso que conseguisse iniciar sessão no sistema visado poderia explorar esta vulnerabilidade e executar código arbitrário com privilégios ao nível do sistema. O intruso poderia então instalar programas, ver, alterar ou eliminar dados, ou ainda criar novas contas com todos os privilégios.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196444">MS10-059</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades na Função de Rastreio para Serviços Poderiam Permitir Elevação de Privilégios (982799)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente e uma vulnerabilidade comunicada de forma privada na Função de Rastreio para Serviços. As vulnerabilidades poderiam permitir elevação de privilégios se um intruso executasse uma aplicação especialmente concebida para o efeito. Um intruso tem que ter credenciais de início de sessão válidas e conseguir iniciar a sessão localmente para explorar esta vulnerabilidade. A vulnerabilidade não poderia ser explorada remotamente ou por utilizadores anónimos.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
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
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                                                 | ID de CVE                                                                        | Avaliação do índice de possibilidade de exploração                                                               | Notas Principais                                                                                                                                                     |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Vulnerabilidade de Corrupção de Memória no Microsoft Silverlight                                          | [CVE-2010-0019](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0019) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-052](http://go.microsoft.com/fwlink/?linkid=194432) | Vulnerabilidade de Sobrecarga de Memória Intermédia no Descodificador de Áudio MPEG Layer-3               | [CVE-2010-1882](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1882) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | Vulnerabilidade de Inicialização de Dados de kernel do Windows                                            | [CVE-2010-1888](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1888) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Vulnerabilidade de Excesso de Número Inteiro em Rede Windows                                              | [CVE-2010-1893](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1893) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Vulnerabilidade de Processamento de Excepção no Win32k                                                    | [CVE-2010-1894](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1894) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | **Esta vulnerabilidade foi divulgada publicamente.**                                                                                                                 |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Vulnerabilidade de Sobrecarga do Conjunto no Win32k                                                       | [CVE-2010-1895](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1895) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Vulnerabilidade de Validação de Intervenção do Utilizador no Win32k                                       | [CVE-2010-1896](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1896) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Vulnerabilidade na Criação de Janelas no Win32k                                                           | [CVE-2010-1897](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1897) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Vulnerabilidade de Delegação do Método Virtual de CLR no Microsoft Silverlight e Microsoft. NET Framework | [CVE-2010-1898](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1898) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Vulnerabilidade de Análise de Registo no Word                                                             | [CVE-2010-1900](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1900) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Vulnerabilidade de Corrupção de Memória no Motor de Análise de RTF no Word                                | [CVE-2010-1901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1901) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-055](http://go.microsoft.com/fwlink/?linkid=194906) | Vulnerabilidade de Descompressão do Codec Cinepak                                                         | [CVE-2010-2553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2553) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-059](http://go.microsoft.com/fwlink/?linkid=196444) | Vulnerabilidade de Corrupção de Memória de Rastreio                                                       | [CVE-2010-2555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2555) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Vulnerabilidade de Corrupção de Memória Não Inicializada                                                  | [CVE-2010-2557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2557) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | Esta vulnerabilidade é mais provável ser explorada no Internet Explorer 6 devido à falta de Prevenção de Execução de Dados como factor atenuante.                    |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Vulnerabilidade de Corrupção de Memória no Processamento de HTML                                          | [CVE-2010-2560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2560) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-057](http://go.microsoft.com/fwlink/?linkid=196275) | Vulnerabilidade de Corrupção de Memória no Excel                                                          | [CVE-2010-2562](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2562) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-050](http://go.microsoft.com/fwlink/?linkid=197103) | Vulnerabilidade de Corrupção de Memória no Movie Maker                                                    | [CVE-2010-2564](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2564) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                                                                                                            |  
| [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393) | Vulnerabilidade de Carregamento de Ícones de Atalhos                                                      | [CVE-2010-2568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2568) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | **Esta vulnerabilidade está a ser explorada actualmente no ecossistema da Internet.**                                                                                |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | Vulnerabilidade de Condição Livre e Dupla no Kernel do Windows                                            | [CVE-2010-1889](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1889) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                            |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Vulnerabilidade de Sobrecarga da Memória Intermédia de Análise de RTF no Word                             | [CVE-2010-1902](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1902) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | O Windows Vista e o Windows 7 são menos susceptíveis a exploração devido aos mecanismos adicionais de atenuação da área dinâmica para dados.                         |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Vulnerabilidade de Corrupção de Memória de Objectos com Ligações a HTML no Word                           | [CVE-2010-1903](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1903) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                            |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Vulnerabilidade de Sobrecarga do Conjunto no SMB                                                          | [CVE-2010-2550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2550) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | É mais provável que exploração resulte em negação de serviço do que em execução de código.                                                                           |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Vulnerabilidade de Corrupção de Memória Não Inicializada                                                  | [CVE-2010-2556](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2556) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                            |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Vulnerabilidade de Corrupção de Memória de Condição Race                                                  | [CVE-2010-2558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2558) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                            |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Vulnerabilidade de Corrupção de Memória Não Inicializada                                                  | [CVE-2010-2559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2559) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                            |  
| [MS10-051](http://go.microsoft.com/fwlink/?linkid=196268) | Vulnerabilidade de Corrupção de Memória no Processamento de Respostas do Msxml2.XMLHTTP.3.0               | [CVE-2010-2561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2561) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                                            |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Vulnerabilidade de Execução Remota de Código em Pedidos de Certificação SChannel Mal Formados             | [CVE-2010-2566](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2566) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | É provável que a exploração resulte em negação de serviço. A execução remota de código é improvável.                                                                 |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Vulnerabilidade de Renegociação de TLS/SSL                                                                | [CVE-2009-3555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3555) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Esta é uma vulnerabilidade de ocultação (spoofing). Foi descrita no [Aviso de Segurança da Microsoft 977377](http://technet.microsoft.com/security/advisory/977377). |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Vulnerabilidade Entre Domínios do Processador de Eventos                                                  | [CVE-2010-1258](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1258) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Trata-se de uma vulnerabilidade ao nível da divulgação de informações.                                                                                               |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Vulnerabilidade de Corrupção de Memória no IPv6                                                           | [CVE-2010-1892](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1892) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Esta é uma vulnerabilidade de "negação de serviço".                                                                                                                  |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Vulnerabilidade de Validação de Variável no SMB                                                           | [CVE-2010-2551](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2551) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Esta é uma vulnerabilidade de "negação de serviço".                                                                                                                  |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Vulnerabilidade de Esgotamento da Pilha no SMB                                                            | [CVE-2010-2552](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2552) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração funcional   | Esta é uma vulnerabilidade de "negação de serviço".                                                                                                                  |
  
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
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=12361875-b453-45e8-852b-90f2727894fd)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ff00381c-e74b-48e5-9dd9-34dbedd906a2)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=dbdbbe5e-2ef9-4704-80c4-27ef28fd95ef)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=08159149-17de-4640-8818-cb7bd4811531)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=bc949915-4e16-4897-a295-2f99102548ab)  
(Crítica)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b489f8c-ada0-4051-8284-0a941c04d2ed)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1662780f-370a-425b-9917-c601eb54a375)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6e5e16f8-c140-4a1d-b898-8417a6bfd4d8)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=5ddb5e34-f97a-47c6-96c8-ba2ed06ccb77)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Crítica)  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e3574047-5ce5-4461-94aa-4eb3258d5e71)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=deeac521-d3a2-4019-8176-c9228e733cf4)  
(Importante)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=b211664b-434d-4626-816f-c77510cfd44d)<sup>[1]</sup>
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
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b44bd67-48e2-497f-9165-42a702e2cc0d)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaffa70c-6f2b-4e66-b1bc-64bdbbbcd34f)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=4d4e8eeb-a0b2-41c6-9ee4-3f4beb44195e)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b7f28d7a-6b27-4059-865b-5fd55edb6299)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=96b7a562-af16-4f0d-840c-838fb12e7419)  
(Crítica)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5296fb82-c446-4681-a9a0-0f80a2e248be)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=f8ae3978-bad6-4201-8357-2d212ab703ef)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd6cc359-e72e-46ec-a08b-763934e3e115)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/my%20documents/release/5cff5d6e-11a5-40ed-92ac-e12d287919e6)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Crítica)  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6c5455e-bc31-4842-aef4-ebff92324323)  
(Importante)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=decb1fe6-adc8-44f7-89c5-f25767f0cefe)<sup>[1]</sup>
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
<th colspan="14">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Nenhum
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
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=32fe91ef-5a8d-4095-90ee-2ca216696b09)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f76d68df-97e5-489c-a5f6-0c378c1f62ae)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=31ce233e-4d2d-404b-84a8-683319ba8ef7)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9c2110ec-7e6c-4e73-9785-0a8196095ea0)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b0370e1e-dedf-4fe8-a06c-0e0f0a674205)  
(Crítica)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8753ae27-60a4-475a-b8bc-6a7764480295)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=772e765d-0502-4b0b-bde8-d4f62b96db64)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=230e8559-e6df-49d5-acb5-b0cd4bde0bf4)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Crítica)  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=59395f00-90f4-4b68-8dd3-03ff611c1bc8)  
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=923de214-c4fa-41e6-8307-2c5a37f13e8e)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4543bcf0-3505-407b-a5a9-6250ece6fbac)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=4d784b57-8564-4e7e-8f61-f897398e7ea5)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fdfad4ca-37c4-4ac5-bebc-a5ad61299503)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d92f5e69-43cf-4615-aa3b-41f9f40bb57b)  
(Crítica)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=fd3e9d06-1f8b-4ef7-84f6-61e85a1767b8)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=863edf45-0d3b-4408-a47c-258dc4a4fd94)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=03804f59-748e-4832-98e4-2d88564bd10a)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Crítica)  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9ef1c600-bb93-4800-81b8-8c64b369c194)  
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
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=63aa5f8a-fe47-4892-b905-b54e4f3b6580)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9ef992c3-96e9-4533-b844-07424a6054b3)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=d87ac8b3-41fb-4cdd-b305-181a0024d85c)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=782e2963-4a52-4a1d-b99a-34ba841038a7)  
(Crítica)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5e730064-8270-4d63-b497-c5ebeddea1fc)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e4f4f8b3-7a39-4d77-a46b-02c86ad159c3)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Crítica)  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f96b8154-9976-41b0-b9d7-d79887fe9364)  
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
<th colspan="14">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Nenhum
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 e Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=52748886-6280-4247-8cbd-f64db229ee66)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aca69406-f795-4398-968f-959fe3a74e89)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbfaadf8-ab38-456c-956a-ea18c64236c9)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=535c563e-cdac-4e3d-96b0-9947ea22deca)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2062566b-8b81-43c2-875d-9c06d4e3fa82)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9087a3aa-aa55-41f6-8c4c-f322e4aa8681)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=60c81415-b61e-44a4-8dd9-cedec99eb70f)  
(Crítica)
</td>
<td style="border:1px solid black;">
Apenas Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 e Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Crítica)  
Apenas Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Crítica)  
Apenas Windows Vista Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4486f97c-4cf8-4236-bfc3-b50e72e2a5c1)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9345207-7242-4b71-bf80-b52031e08f8c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=8aded9dd-08d6-4b19-955f-0d8414868cf9)<sup>[1]</sup>
(Importante)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=a1d8ed0d-a3b5-416a-ab8b-77501da62132)<sup>[2]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4684c4df-0a5c-4dba-82e5-059378737118)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 e Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dfb31aa2-7457-4581-9e28-7984a360edf4)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=37648e95-05c2-4802-9a0f-660200baa229)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2835ed1-5ca6-4347-8ff1-e694b1ac49ff)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=577131cd-1229-4746-89d7-84d75f29e1f0)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=cd1185e3-ca22-4197-a53b-e7a2806ac352)  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=65b04e29-8e39-46de-94e8-b653969b1ffd)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=10c9d5f1-53ed-459b-a663-e69bdb845a6b)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=469b732d-ca62-4a48-bb55-99f2ae4ddcf5)  
(Crítica)
</td>
<td style="border:1px solid black;">
Apenas Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 e Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Crítica)  
Apenas Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Crítica)  
Apenas Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b547898e-f8a9-49dc-b49d-cffec5a001bc)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1620e7ac-3913-478d-8120-e9f46d98f453)  
(Importante)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=4baff9ae-dd25-4942-b45e-f281d0e1f4ac)<sup>[1]</sup>
(Importante)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=0a226592-8f98-4f67-ac60-1d00cbc56598)<sup>[2]</sup>
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18152cd4-815f-425f-8694-fbabcbe80609)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=110f932f-d13c-4486-a295-e6068d5d8d7a)  
(Importante)
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
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3aabd189-7d4c-4c9f-8854-f33127b1c309)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e0253d4-f0c0-4f28-ba08-6907c2fcb339)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=73b5f45c-c9d6-491f-8483-98838b2a7c04)\*  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8239cb9e-bb5a-4157-8038-33d0b329eaee)\*\*  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=409b9298-1e7d-48cf-9872-ffbdc56ebe53)\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a94e2e38-116a-4b63-9328-6c33e63bbbfe)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Windows Server 2008 apenas para sistemas de 32 bits:  
[Microsoft .NET Framework 2.0 Service Pack 1 e Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Crítica)  
Windows Server 2008 apenas para sistemas de 32 bits:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Crítica)  
Apenas Windows Server 2008 para sistemas de 32 bits Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=611765ab-b3f3-45db-92b2-ee040b9cfd27)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8b1a3f7-7147-494e-bfc0-b1979b9578e6)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=844404be-f2e8-47bc-9650-9e2bbe383814)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4c9b3e60-e166-40c9-8938-3cba0a399c47)\*  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29c6fc2d-d318-4a63-9ab2-82e84272aaf2)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a96891ff-8771-47b3-81bb-8640adb6c098)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=43ece408-4aa7-4819-b3f6-7f0719ed3213)\*  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5ef8abf0-c89e-4911-8d77-42400d9a398f)\*\*  
(Crítica)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9b869bab-0797-4f83-8c64-23dda9983c8d)\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=602dd3f6-0d09-4546-b1db-d7b6b04edb66)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Windows Server 2008 apenas para sistemas baseados em x64:  
[Microsoft .NET Framework 2.0 Service Pack 1 e Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Crítica)  
Windows Server 2008 apenas para sistemas baseados em x64:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Crítica)  
Apenas Windows Server 2008 para sistemas baseados em x64 Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=131f3512-1585-462e-a4f1-3f359aac44bd)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1c25cb7-7e82-4c14-9666-aff52dd308b4)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=08491c73-66b1-4c4c-8740-ea596a730fc1)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fa84e547-2190-402f-9467-2450deeff565)\*  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cfe227b5-6660-49f8-9d71-a997dd83de0b)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b16a422-0ee9-4eab-9cfe-e7688ffa0d76)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=b6faee94-e821-432d-bfa2-9008664566af)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2f1eee63-2cca-4ec5-b196-36de3c0054cf)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=24d8f0a3-51a9-46c1-b870-a2239bf600e4)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Windows Server 2008 apenas para sistemas baseados em Itanium:  
[Microsoft .NET Framework 2.0 Service Pack 1 e Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Crítica)  
Windows Server 2008 apenas para sistemas baseados em Itanium:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Crítica)  
Apenas Windows Server 2008 para sistemas baseados em Itanium Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 e Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=972efd3a-ec1e-49b2-835e-76f4b21b5b79)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=45fe5135-aa89-4f60-8cdb-ec0edc9a7e77)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8aa12902-c234-4fd9-bba3-6767eafc38fc)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=84f89dca-108c-4956-9aa2-866e17a872fc)  
(Importante)
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
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 para sistemas de 32 bits
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=22e62b5c-e4c1-47d0-ae4a-8bd2d70d0a0a)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=71716507-7080-4102-991e-6afc7cc377d5)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=31d0f5ac-2cff-42a1-8f18-128bbfc4e57d)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ecaf42e0-a288-40c1-8602-21e967a87408)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=8d58ebc4-a5f9-4318-a6f1-168c1bcdae3c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=2e782ac9-b5d5-490e-a01a-7d4481eab224)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=a7d60864-5942-47ed-a6f3-1c07b4833a14)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=68bddf4b-b597-477e-80e4-9293d7160496)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=3a5a088e-644a-4a0e-9a09-0370bcd97688)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits](http://www.microsoft.com/downloads/details.aspx?familyid=ce6233f3-2ee5-4329-908d-ba9b28ecc553)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=9499f771-c388-4de3-a5c7-8cc8b00b4395)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=c457d8ec-83b7-446f-b77c-e47d4187e616)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=a4f6d7c2-b475-4900-82f0-75f5be0b7b63)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ca57a47a-9111-4abe-9356-4962ca2c1d65)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=ad1ddf94-d714-4b36-8256-42bf79d03a90)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=24751193-592f-4c44-a8d6-f4112d4f011b)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=b00ec47c-402e-4207-a4c9-6c1900f254f8)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=5ff09e03-d662-4b23-ab26-d25ca2ba58df)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=163fe2bd-f999-47c1-9a35-c4fc868bda51)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=146270fa-cd6f-440a-aa3e-e93af0bff447)  
(Importante)
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=0d9dd09b-db40-462b-88b0-4dbb8180e81f)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=c9aeea25-ca14-4b42-9018-a27c9d8899c4)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=a48cdac5-4d78-49b5-a6d8-ecf6c58cace2)\*  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e7757bbc-3ef0-421d-ab57-0083a302c77b)\*\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=52642a8d-1081-4496-848e-9b03baf3fdac)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)\*  
(KB983590)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=c1ad1248-07f1-42d4-baa4-8a20837ec7b4)\*  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=6bbc9cb1-0b59-4473-adf9-2ce2f0f94c0a)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=a1f95600-34e5-44b3-b2cb-b2b2cbf645cb)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=333fb6e4-f867-4dcb-beb3-2d88e428ca2e)\*  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ce2bb5d4-f661-44e3-ac28-0b81f7b72670)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b7c2e91f-ca8a-4237-99c8-ca53c91cf73e)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=b4d3210e-f3ad-4dbb-9390-6e98eeb99eaa)  
(Moderada)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7b457d04-03a9-4eb0-ba6a-ab45267e4f74)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=783fb42c-3698-4b1d-a692-3ff319578931)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f23dec0f-a33b-4d8c-a86d-0e9368ae7ff5)  
(Moderada)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2543191a-09cb-4417-bbb2-aac4d9a2a756)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c3cd7f2f-e198-4fbd-a65d-21a1bf51eb61)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=62034ecb-a6bd-46c5-a03d-9642880bc2d6)  
(Importante)
</td>
</tr>
</table>
 
**Notas para o Windows Server 2008 e Windows Server 2008 R2**

**\*Instalação Server Core afectada.** Esta actualização aplica-se, com a mesma classificação de gravidade, a edições suportadas do Windows Server 2008 ou Windows Server 2008 R2, conforme indicado, quer a instalação tenha sido efectuada ou não utilizando a opção de instalação Server Core. Para mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx)e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 e Windows Server 2008 R2 como indicado, se estes tiverem sido instalados usando a opção de instalação Server Core. Para mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx)e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Notas para o MS10-050**

<sup>[1]</sup>Estas versões do Windows Movie Maker são fornecidas com os sistemas operativos indicados.

<sup>[2]</sup>O Windows Movie Maker 2.6 é uma transferência opcional que pode ser instalada nos sistemas operativos indicados.

**Nota para o MS10-060**

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=978eb887-25b6-4dde-a2ec-d2d1e7f1a434)  
(KB2251389)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=032e1530-8736-4e1c-a704-967679227619)  
(KB2264397)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4360bcec-0731-4d4a-89eb-7d28a4607f06)  
(KB2251399)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7cecbce3-bbb7-47d1-bda3-64d7e0f69f62)  
(KB2264403)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0d7210a3-662e-41e7-affc-ae94f9d89388)<sup>[1]</sup>
(KB2251419)  
(Crítica)
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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 para Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Importante)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Conversor de Formato de Ficheiros Open XML para Mac
</td>
<td style="border:1px solid black;">
[Conversor de Formato de Ficheiros Open XML para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
(Importante)
</td>
<td style="border:1px solid black;">
[Conversor de Formato de Ficheiros Open XML para Mac](http://www.microsoft.com/downloads/details.aspx?familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=39fe2229-9201-4270-bdc1-20bc8e30a766)  
(KB2251437)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ed5b9671-651d-41f3-aed3-93ee8a28657f)  
(KB2277947)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=feb121ad-e5f6-40e2-bf12-045ae5c2a754)  
(KB2092914)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
</table>
 
**Nota para o MS10-056**

<sup>[1]</sup>Para o Microsoft Office Word 2007 Service Pack 2, para além do pacote de actualização de segurança KB2251419, os clientes têm também de instalar a actualização de segurança para o Pack de Compatibilidade do Microsoft Office para formatos de ficheiros Word, Excel e PowerPoint 2007 Service Pack 2 (KB2277947) para estarem protegidos contra as vulnerabilidades descritas no MS10-056.

#### Software e Ferramentas de Desenvolvimento da Microsoft

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
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
Microsoft Silverlight 2
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> quando instalado em Mac  
(KB982926)  
(Crítica)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> quando instalado em todas as edições de clientes Microsoft Windows  
(KB982926)  
(Crítica)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> quando instalado em todas as edições de servidores Microsoft Windows\*\*  
(KB982926)  
(Crítica)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 3
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> quando instalado em Mac  
(KB978464)  
(Crítica)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> quando instalado em todas as edições de clientes Microsoft Windows  
(KB978464)  
(Crítica)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> quando instalado em todas as edições de servidores Microsoft Windows\*\*  
(KB978464)  
(Crítica)
</td>
</tr>
</table>
 
**Notas para o MS10-060**

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 e Windows Server 2008 R2 como indicado, se estes tiverem sido instalados usando a opção de instalação Server Core. Para mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx)e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

<sup>[1]</sup>Esta transferência actualiza o Microsoft Silverlight 2 para uma versão mais recente do Microsoft Silverlight que não é afectada pelas vulnerabilidades descritas no boletim.

<sup>[2]</sup>Esta actualização actualiza o Microsoft Silverlight para uma compilação mais recente que não é afectada pelas vulnerabilidades descritas no boletim.

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

Orientações e ferramentas de detecção e implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para mais informações, visite o [Centro de Gestão de Actualizações TechNet](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em Casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem na opção para obter as actualizações de segurança mais recentes.

As actualizações de segurança estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt) e no [Windows Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt). As actualizações de segurança estão também disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".

Finalmente, as actualizações de segurança podem ser transferidas a partir do [Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). O Catálogo do Microsoft Update permite pesquisar conteúdos disponibilizados através do Windows Update e do Microsoft Update, incluindo actualizações de segurança, controladores e service packs. Utilizando o número do boletim de segurança para pesquisar (por exemplo, "MS07-036"), pode adicionar todas as actualizações aplicáveis ao seu cesto (incluindo diferentes idiomas para uma actualização) e transferi-las para uma pasta à sua escolha. Para mais informação sobre o Catálogo do Microsoft Update, consulte as [Perguntas Mais Frequentes sobre o Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Nota** Desde 1 de Agosto de 2009, a Microsoft deixou de prestar suporte para o Office Update e a ferramenta Office Update Inventory Tool. Para continuar a obter as mais recentes actualizações para produtos Microsoft Office, utilize o [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt). Para mais informações, consulte [Acerca do Microsoft Office Update: Perguntas Mais Frequentes](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx).

**Orientações de Detecção e Implementação**

A Microsoft fornece orientações sobre detecção e implementação de actualizações de segurança. Estas orientações contêm recomendações e informação que podem auxiliar os profissionais de TI a compreender como utilizar as diversas ferramentas para detecção e implementação de actualizações de segurança. Para obter mais informações, consulte o [Artigo 961747 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/961747).

**Microsoft Baseline Security Analyzer**

O Microsoft Baseline Security Analyzer (MBSA) permite aos administradores procurar actualizações de segurança em falta e comuns erros de configuração de segurança em sistemas locais e remotos. Para obter mais informações acerca do MBSA, visite o Web site do [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

O Windows Server Update Services (WSUS) permite que os administradores de tecnologia de informação implementem as actualizações mais recentes de produtos da Microsoft em computadores que estejam a executar o sistema operativo Windows. Para mais informações sobre como implementar actualizações de segurança usando o Windows Server Update Services, consulte o artigo TechNet sobre o [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

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

As [Orientações de Segurança para Gestão de Actualizações](http://go.microsoft.com/fwlink/?linkid=21168)fornecem informações adicionais referentes a recomendações de melhores práticas da Microsoft para a aplicação de actualizações de segurança.

**Obter Outras Actualizações de Segurança**

Estão disponíveis actualizações para outros problemas de segurança nas seguintes localizações:

-   As actualizações de segurança estão disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".
-   As actualizações para plataformas de consumidor estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt).
-   Pode obter as actualizações de segurança oferecidas no Windows Update este mês no ficheiro de imagem de CD em formato ISO com as informações de segurança e críticas no Centro de Transferências. Para mais informações, consulte o [Artigo 913086 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/913086).

**IT Pro Security Community**

Aprenda a melhorar a segurança, optimize a sua infra-estrutura informática e participe em tópicos de segurança juntamente com outros profissionais de informática no Web site [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Agradecimentos

A Microsoft [agradece](http://go.microsoft.com/fwlink/?linkid=21127) às seguintes entidades por trabalharem connosco para proteger os clientes:

-   Sergey I. Ulasen e Oleg Kupreev, da [VirusBlokAda](http://www.anti-virus.by/), por fornecerem informações sobre uma questão descrita no boletim MS10-046
-   Andreas Marx e Maik Morgenstern, da [AV-Test](http://www.av-test.org/), por fornecerem informações sobre uma questão descrita no boletim MS10-046
-   Will Dormann, da [CERT/CC](http://www.cert.org), por trabalhar connosco numa questão descrita no boletim MS10-046
-   Niels Teusink, por trabalhar connosco numa questão descrita no boletim MS10-046
-   Stefan Kanthak, por trabalhar connosco numa questão descrita no boletim MS10-046
-   Tavis Ormandy, da [Google Inc.](http://www.google.com/), por fornecer informações sobre três questões descritas no boletim MS10-047
-   Tavis Ormandy, da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS10-048
-   Matthieu Suiche, da [MoonSols](http://moonsols.com/), por fornecer informações sobre duas questões descritas no boletim MS10-048
-   Matthieu Suiche, da [MoonSols](http://moonsols.com/), por trabalhar connosco nas alterações a nível da protecção defensiva profunda no boletim MS10-048
-   Nicolás Economou, da [Core Security Technologies](http://www.coresecurity.com/), por fornecer informações sobre uma questão descrita no boletim MS10-048
-   Marsh Ray e Steve Dispensa, da [PhoneFactor](http://www.phonefactor.com/), por fornecer informações sobre uma questão descrita no boletim MS10-049
-   Dyon Balding, da [Secunia](http://secunia.com/), por fornecer informações sobre uma questão descrita no boletim MS10-050
-   SkyLined, da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS10-051
-   Moritz Jodeit, da n.runs AG, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint's](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-052
-   David Bloom, da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS10-053
-   Nicolas Joly, da [Equipa de Investigação de Vulnerabilidades da VUPEN](http://www.vupen.com), por fornecer informações sobre uma questão descrita no boletim MS10-053
-   Gambino ZaDarkSide por fornecer informações sobre uma questão descrita no boletim MS10-053
-   Laurent Gaffié, da [stratsec](http://www.stratsec.net/), por fornecer informações sobre uma questão descrita no boletim MS10-054
-   Todd Wease e Richard Johnson, da [Sourcefire VRT](http://www.sourcefire.com/services/sf_vrt.html), por fornecer informações sobre uma questão descrita no boletim MS10-054
-   Riku Hietamaki e Joshua Morin, da [Codenomicon](http://www.codenomicon.com/), por fornecer informações sobre uma questão descrita no boletim MS10-054
-   Investigador anónimo, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-055
-   L.W.Z, da [team509](http://www.team509.com/), a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-056
-   Wushi, da [team509](http://www.team509.com/), a trabalhar com a [VeriSign iDefense Labs](http://labs.idefense.com/), por fornecer informações sobre uma questão descrita no boletim MS10-056
-   [team509](http://www.team509.com/), a trabalhar com a[VeriSign iDefense Labs](http://labs.idefense.com/), por fornecer informações sobre uma questão descrita no boletim MS10-056
-   Rodrigo Rubira Branco, da Equipa de Investigação IPS da [Check Point](http://www.checkpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-056
-   Investigador anónimo, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-056
-   Damián Frizza, da [Core Security Technologies](http://www.coresecurity.com/), por fornecer informações sobre uma questão descrita no boletim MS10-057
-   Darren Willis, da [Fourteenforty Research Institute, Inc.](http://www.fourteenforty.jp/), por fornecer informações sobre uma questão descrita no boletim MS10-058
-   Matthieu Suiche, da [MoonSols,](http://moonsols.com/) por fornecer informações sobre uma questão descrita no boletim MS10-058
-   Cesar Cerrudo, da [Argeniss](http://www.argeniss.com/), por fornecer informações sobre uma questão descrita no boletim MS10-059
-   Carsten Book, da , por fornecer informações sobre uma questão descrita no boletim MS10-060
-   [Eamon Nerbonne](http://eamon.nerbonne.org/) por fornecer informações sobre uma questão descrita no boletim MS10-060

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (2 de Agosto de 2010): Publicação do Resumo dos Boletins.
-   V2.0 (10 de Agosto de 2010): Adicionados os boletins MS10-047 a MS10-060.
-   V2.1 (1 de Setembro de 2010): Adicionada uma nota ao MS10-056 para informar os clientes que utilizam o Word 2007 que, para além do pacote da actualização de segurança KB2251419, têm também de instalar o pacote da actualização de segurança KB2277947.

*Built at 2014-04-18T01:50:00Z-07:00*
