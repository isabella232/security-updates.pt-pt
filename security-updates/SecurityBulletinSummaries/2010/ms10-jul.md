---
TOCTitle: 'MS10-JUL'
Title: Resumo dos Boletins de Segurança Microsoft de Julho 2010
ms:assetid: 'ms10-jul'
ms:contentKeyID: 61235158
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms10-jul(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Julho 2010
========================================================

Data de publicação: 13 de julho de 2010 | Updated: 14 de julho de 2010

**actualizada:** 1.1

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Julho de 2010.

Com a publicação dos boletins de Julho de 2010, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 8 de Julho de 2010. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 14 de Julho de 2010, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o Webcast de boletins de segurança de Julho](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032454299&culture=en-us). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194729">MS10-042</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Centro de Ajuda e Suporte Poderia Permitir Execução Remota de Código (2229593)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade divulgada publicamente na funcionalidade do Centro de Ajuda e Suporte do Windows que é fornecida com as edições suportadas do Windows XP e do Windows Server 2003. Esta vulnerabilidade poderia permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito com um browser da Web ou se clicasse numa hiperligação especialmente concebida para o efeito presente numa mensagem de correio electrónico. A vulnerabilidade não pode ser automaticamente explorada através de correio electrónico. Para um ataque poder ser bem sucedido, é necessário que um utilizador clique numa hiperligação listada numa mensagem de correio electrónico.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194164">MS10-043</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Canonical Display Driver Poderia Permitir Execução Remota de Código (2032276)</strong><br />
<br />
Esta actualização de segurança corrige uma vulnerabilidade divulgada publicamente no Canonical Display Driver (cdd.dll). Embora a vulnerabilidade possa permitir execução de código, é improvável que a execução de código seja bem sucedida devido à aleatoriedade de memória. Na maior parte dos cenários, é bastante mais provável que um intruso que conseguisse tirar partido desta vulnerabilidade pudesse fazer com que o sistema afectado deixasse de responder e fosse automaticamente reiniciado.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=195244">MS10-044</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades nos Controlos ActiveX do Microsoft Office Access Poderiam Permitir Execução Remota de Código (982335)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades comunicadas de forma privada nos Controlos ActiveX do Microsoft Office Access. As vulnerabilidades poderiam permitir a execução remota de código se um utilizador abrisse um ficheiro Office especialmente concebido para o efeito ou visualizasse uma página Web que instanciasse controlos ActiveX do Access. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=178810">MS10-045</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft Office Outlook Poderia Permitir Execução Remota de Código (978212)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um utilizador abrisse um anexo contido numa mensagem de correio electrónico especialmente concebida para o efeito usando uma versão afectada do Microsoft Office Outlook. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
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
A tabela que se segue fornece uma avaliação da possibilidade de exploração para cada uma das vulnerabilidades abordadas este mês. As vulnerabilidades encontram-se listadas por ordem decrescente de nível de avaliação da possibilidade de exploração e, depois, por ID de CVE. Apenas são incluídas as vulnerabilidades às quais foi atribuída uma classificação de gravidade Crítica ou Importante nos boletins.
  
**Como utilizar esta tabela?**
  
Utilize esta tabela para saber mais sobre a probabilidade de códigos de exploração funcionais serem lançados no espaço de 30 dias após o lançamento do boletim de segurança, para cada uma das actualizações de segurança que poderá ter de instalar. Deverá rever cada avaliação em baixo, conforme a sua configuração específica, para dar prioridade à sua implementação. Para obter mais informações sobre o significado destas classificações e sobre como elas são estabelecidas, consulte o [Índice de Possibilidade de Exploração da Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                | ID de CVE                                                                        | Avaliação do índice de possibilidade de exploração                                                               | Notas Principais                                                                     |  
|-----------------------------------------------------------|--------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|  
| [MS10-045](http://go.microsoft.com/fwlink/?linkid=178810) | Vulnerabilidade em Anexos SMB no Microsoft Outlook                       | [CVE-2010-0266](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0266) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                            |  
| [MS10-044](http://go.microsoft.com/fwlink/?linkid=195244) | Vulnerabilidade em Controlos ActiveX do Access                           | [CVE-2010-0814](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0814) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                            |  
| [MS10-044](http://go.microsoft.com/fwlink/?linkid=195244) | Vulnerabilidade de Variável Não Inicializada ACCWIZ.dll                  | [CVE-2010-1881](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1881) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | (Nenhuma)                                                                            |  
| [MS10-042](http://go.microsoft.com/fwlink/?linkid=194729) | Vulnerabilidade de Validação de URL no Centro de Ajuda                   | [CVE-2010-1885](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1885) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | **Esta vulnerabilidade está a ser explorada actualmente no ecossistema da Internet** |  
| [MS10-043](http://go.microsoft.com/fwlink/?linkid=194164) | Vulnerabilidade de Excesso de Número Inteiro no Canonical Display Driver | [CVE-2009-3678](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3678) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                            |
  
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
</tr>
<tr>
<th colspan="3">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-042**](http://go.microsoft.com/fwlink/?linkid=194729)
</td>
<td style="border:1px solid black;">
[**MS10-043**](http://go.microsoft.com/fwlink/?linkid=194164)
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
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 2 e Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 e Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7c2122bb-0ecf-4467-a3ba-6fb862f603c5)  
(Crítica)
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
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9232a336-9ded-4820-bac4-2d68877ee76c)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-042**](http://go.microsoft.com/fwlink/?linkid=194729)
</td>
<td style="border:1px solid black;">
[**MS10-043**](http://go.microsoft.com/fwlink/?linkid=194164)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Baixa**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cd4363b2-d7a7-4fff-8bcd-6fd02bd1ac07)  
(Baixo)
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
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a6bafd3b-c921-466d-bee0-59a3fe126712)  
(Baixo)
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
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b61cc2d5-8432-4681-aa2c-a8807ec1fcf4)  
(Baixo)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
<tr>
<th colspan="3">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-042**](http://go.microsoft.com/fwlink/?linkid=194729)
</td>
<td style="border:1px solid black;">
[**MS10-043**](http://go.microsoft.com/fwlink/?linkid=194164)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 para sistemas de 32 bits
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
Windows 7 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=33ec8c0e-1617-46bf-bd7f-2ce750f89d7f)  
(Crítica)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-042**](http://go.microsoft.com/fwlink/?linkid=194729)
</td>
<td style="border:1px solid black;">
[**MS10-043**](http://go.microsoft.com/fwlink/?linkid=194164)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
Nenhum
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64](http://www.microsoft.com/downloads/details.aspx?familyid=2a9998fc-beac-4ccf-aa61-4232106adae1)\*\*\*  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
</tr>
</table>
 
**Nota para o Windows Server 2008 R2**

**\*\*\*Instalação Server Core não afectada.** A vulnerabilidade resolvida por esta actualização não afecta as edições suportadas do Windows Server 2008 R2 como indicado, quando instalado utilizando a opção de instalação Server Core, embora possam estar presentes no sistema ficheiros afectados por esta vulnerabilidade. Contudo, os utilizadores com ficheiros afectados continuarão a receber esta actualização porque os ficheiros actualizados são mais recentes (com números de versão superiores) do que os ficheiros actualmente no seu sistema. Para obter mais informações sobre esta opção de instalação, consulte os artigos MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) e [Server Core para Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e do Windows Server 2008 R2; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS10-044**](http://go.microsoft.com/fwlink/?linkid=195244)
</td>
<td style="border:1px solid black;">
[**MS10-045**](http://go.microsoft.com/fwlink/?linkid=178810)
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
Não aplicável
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=daacf400-4aa3-4479-a60f-b8863ba1e16d)  
(KB980371)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=93768ac6-e6d7-4175-a6e3-666210494678)  
(KB981716)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ef5b0048-96f1-43a6-9848-7f6adccd10b3)  
(KB980373)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 1 e Microsoft Office System 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2007 Service Pack 1 e Microsoft Office Access 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=af2862e2-da37-4cbe-8974-e517eb666f14)  
(KB979440)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2007 Service Pack 1 e Microsoft Office Outlook 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e2e7c49-6665-4135-adbb-8e831a91d0fe)  
(KB980376)  
(Importante)
</td>
</tr>
</table>
 

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

-   David Hansel, da [Reactive Systems, Inc](http://www.reactive-systems.com/), por fornecer informações sobre uma questão descrita no boletim MS10-043
-   Investigador anónimo, a trabalhar com a [Zero Day Initiative](http://www.zerodayinitiative.com/) da [TippingPoint](http://www.tippingpoint.com/), por fornecer informações sobre uma questão descrita no boletim MS10-044
-   Robert Freeman, da [IBM ISS X-Force](http://www.iss.net/), por fornecer informações sobre uma questão descrita no boletim MS10-044
-   Yorick Koster, a trabalhar com o [programa SSD/SecuriTeam Secure Disclosure](http://www.beyondsecurity.com/ssd.html), por fornecer informações sobre uma questão descrita no boletim MS10-045

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (13 de Julho de 2010): Publicação do Resumo dos Boletins.
-   V1.1 (14 de Julho de 2010): Removida uma referência errada ao Windows Embedded Standard 7 para o MS10-043.

*Built at 2014-04-18T01:50:00Z-07:00*
