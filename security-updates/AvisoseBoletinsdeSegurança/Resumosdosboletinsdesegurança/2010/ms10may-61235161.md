---
TOCTitle: 'MS10-MAY'
Title: Resumo dos Boletins de Segurança Microsoft de Maio 2010
ms:assetid: 'ms10-may'
ms:contentKeyID: 61235161
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms10-may(v=Security.10)'
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Maio 2010
=======================================================

Data de publicação: 11 de maio de 2010 | Updated: 19 de maio de 2010

**actualizada:** 1.2

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Maio de 2010.

Com a publicação dos boletins de Maio de 2010, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 6 de Maio de 2010. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 12 de Maio de 2010, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o webcast de boletins de segurança de Maio](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032427724&culture=en-us). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=188377">MS10-030</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Outlook Express e no Windows Mail Poderia Permitir a Execução Remota de Código (978542)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Outlook Express, Windows Mail e Windows Live Mail, comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se um utilizador visitasse um servidor de correio electrónico malicioso. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=178811">MS10-031</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft Visual Basic for Applications Poderia Permitir Execução Remota de Código (978213)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Visual Basic for Applications, comunicada de forma privada. A vulnerabilidade poderia permitir a execução remota de código se uma aplicação anfitriã abrisse e passasse um ficheiro especialmente concebido para o efeito para o runtime do Visual Basic for Applications. Se um utilizador tiver sessão iniciada com privilégios administrativos, um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter controlo total sobre um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Office, Microsoft Visual Basic for Applications</td>
</tr>
</tbody>
</table>
  
Índice de possibilidade de exploração  
-------------------------------------
  
<span></span>
A tabela que se segue fornece uma avaliação da possibilidade de exploração para cada uma das vulnerabilidades abordadas este mês. As vulnerabilidades encontram-se listadas por ordem decrescente de nível de avaliação da possibilidade de exploração e, depois, por ID de CVE. Apenas são incluídas as vulnerabilidades às quais foi atribuída uma classificação de gravidade Crítica ou Importante nos boletins.
  
**Como utilizar esta tabela?**
  
Utilize esta tabela para saber mais sobre a probabilidade de códigos de exploração funcionais serem lançados no espaço de 30 dias após o lançamento do boletim de segurança, para cada uma das actualizações de segurança que poderá ter de instalar. Deverá rever cada avaliação em baixo, conforme a sua configuração específica, para dar prioridade à sua implementação. Para obter mais informações sobre o significado destas classificações e sobre como elas são estabelecidas, consulte o [Índice de Possibilidade de Exploração da Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                         | ID de CVE                                                                        | Avaliação do índice de possibilidade de exploração                                                               | Notas Principais                                                                                                                             |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-031](http://go.microsoft.com/fwlink/?linkid=178811) | Vulnerabilidade de Corrupção na Memória de Pilha VBE6.DLL                         | [CVE-2010-0815](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0815) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | (Nenhuma)                                                                                                                                    |  
| [MS10-030](http://go.microsoft.com/fwlink/?linkid=188377) | Vulnerabilidade de Excesso de Número Inteiro no Outlook Express e no Windows Mail | [CVE-2010-0816](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0816) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | A exploração no Windows Vista e em sistemas operativos posteriores é menos provável devido a factores atenuantes na área dinâmica para dados |
  
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
</tr>
<tr>
<th colspan="2">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://go.microsoft.com/fwlink/?linkid=188377)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 5.5 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=661f5de3-a593-4961-8e8d-2777797eb5c5)  
(KB978542)  
(Crítica)  
[Microsoft Outlook Express 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cda75174-b535-4559-a52d-b5ec3a1df349)  
(KB978542)  
(Crítica)
</td>
</tr>
<tr>
<th colspan="2">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://go.microsoft.com/fwlink/?linkid=188377)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 e Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=99707c3d-a3cb-47da-b38e-8ae0227fd703)  
(KB978542)  
(Crítica)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=99707c3d-a3cb-47da-b38e-8ae0227fd703)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=44bc97bb-6f76-4c96-af72-69daaea80fff)  
(KB978542)  
(Crítica)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=44bc97bb-6f76-4c96-af72-69daaea80fff)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<th colspan="2">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://go.microsoft.com/fwlink/?linkid=188377)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Classificação de Gravidade Agregada**
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=eb9742fc-0934-4b38-9ec4-3597fc71ec00)  
(KB978542)  
(Crítica)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=5678515a-97ea-4e00-8700-d3f2fcdc0efc)  
(KB978542)  
(Crítica)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=60ef635b-cb6d-402f-b904-e69b519d797f)  
(KB978542)  
(Crítica)
</td>
</tr>
<tr>
<th colspan="2">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://go.microsoft.com/fwlink/?linkid=188377)
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
Windows Vista Service Pack 1 e Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=a970c869-24fe-4ef4-b189-7a6bac2411f1)  
(KB978542)  
(Crítica)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=a970c869-24fe-4ef4-b189-7a6bac2411f1)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 e Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=9a7853b5-4f9f-4467-9530-eea2efd504a5)  
(KB978542)  
(Crítica)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=9a7853b5-4f9f-4467-9530-eea2efd504a5)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<th colspan="2">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://go.microsoft.com/fwlink/?linkid=188377)
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
Windows Server 2008 para sistemas de 32 bits e Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=5f77a640-247c-4ed2-9fca-4b7344f4dc7c)\*\*  
(KB978542)  
(Crítica)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=5f77a640-247c-4ed2-9fca-4b7344f4dc7c)\*\*<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em x64 e Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=b0eab011-5847-44e4-bc0d-5c5355e1e8d0)\*\*  
(KB978542)  
(Crítica)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=b0eab011-5847-44e4-bc0d-5c5355e1e8d0)\*\*<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium e Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=da01ae82-895e-4739-916f-a63b9095a076)  
(KB978542)  
(Crítica)  
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=da01ae82-895e-4739-916f-a63b9095a076)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<th colspan="2">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://go.microsoft.com/fwlink/?linkid=188377)
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
Windows 7 para sistemas de 32 bits
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=1f0c17be-ba4c-4a1c-b9c3-8ac368800947)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=a70f15e1-512c-44ca-a308-928e237ac0ce)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<th colspan="2">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-030**](http://go.microsoft.com/fwlink/?linkid=188377)
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
Windows Server 2008 R2 para sistemas baseados em x64
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=e2e25c02-38ce-4868-a01a-39fc7d2a4150)\*\* <sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Windows Live Mail](http://www.microsoft.com/downloads/details.aspx?familyid=53ed1055-b5ee-4fde-9550-f8b401916467)<sup>[1]</sup>
(KB978542)  
(Importante)
</td>
</tr>
</table>
 
**Nota para o Windows Server 2008 e Windows Server 2008 R2**

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 e Windows Server 2008 R2 como indicado, se estes tiverem sido instalados usando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) e [Server Core para Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e do Windows Server 2008 R2; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Nota para o MS10-030**

<sup>[1]</sup>O Windows Live Mail é um componente fora do ciclo regular deste sistema operativo que necessita de ser instalado separadamente para que a vulnerabilidade exista.

#### Suites e Software do Microsoft Office

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Suites, Sistemas e Componentes do Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-031**](http://go.microsoft.com/fwlink/?linkid=178811)
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
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=72c23b0f-4e24-4334-bc8a-334adc8bc42b)<sup>[1]</sup>   
(KB976380)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f8eac9bc-8389-4ac8-8b29-9a8180d9fd34)<sup>[1]</sup>   
(KB976382)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office System 2007 Service Pack 1 e Microsoft Office System 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=160ad53e-6475-4550-90c2-444e4abea730)<sup>[1]</sup>   
(KB976321)  
(Importante)
</td>
</tr>
</table>
 
**Notas para o MS10-031**

<sup>[1]</sup>Estas actualizações para o Microsoft Office aplicam-se a todas as suites suportadas do Microsoft Office e a outro software Microsoft Office que contenha o componente do Office partilhado vulnerável. Isto inclui, para além de outras possíveis, versões suportadas do Microsoft Office Visio e do Microsoft Office Project.

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

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
Microsoft Visual Basic for Applications
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS10-031**](http://go.microsoft.com/fwlink/?linkid=178811)
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
Microsoft Visual Basic for Applications
</td>
<td style="border:1px solid black;">
[Microsoft Visual Basic for Applications](http://www.microsoft.com/downloads/details.aspx?familyid=436a8a66-352e-44d1-a610-c825083ad24a)<sup>[1]</sup>
(KB974945)  
(Crítica)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Basic for Applications SDK
</td>
<td style="border:1px solid black;">
Microsoft Visual Basic for Applications SDK<sup>[2]</sup><sup>[3]</sup>
(Crítica)
</td>
</tr>
</table>
 
**Notas para o MS10-031**

<sup>[1]</sup>Este pacote de actualização aplica-se às versões suportadas do runtime do Microsoft Visual Basic for Applications (Vbe6.dll) e apenas está disponível no Centro de Transferências da Microsoft.

<sup>[2]</sup>As versões suportadas do VBA SDK são o Microsoft Visual Basic for Applications SDK 6.3, o Microsoft Visual Basic for Applications SDK 6.4 e o Microsoft Visual Basic for Applications SDK 6.5.

<sup>[3]</sup>A versão actualizada do Visual Basic for Applications SDK que resolve a vulnerabilidade descrita neste boletim está disponível na [Summit Software Company](http://www.summsoft.com/) para fornecedores de software independentes (ISV).

Ver também outras categorias de software nesta secção, **Localizações do Software Afectado e das Transferências**, para mais ficheiros de actualização com o mesmo identificador do boletim. Este boletim abrange mais de uma categoria de software.

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

-   Francis Provencher, da Protek Research Lab, por fornecer informações sobre uma questão descrita no boletim MS10-030
-   [NSFocus Security Team](http://www.nsfocus.com/), por fornecer informações sobre uma questão descrita no boletim MS10-031

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (11 de Maio de 2010): Publicação do Resumo dos Boletins.
-   V1.1 (12 de Maio de 2010): Correcção dos requisitos de reinício para o MS10-030.
-   V1.2 (19 de Maio de 2010): Remoção de referências erradas ao Windows Mail quando instalado no Windows 7 e no Windows Server 2008 R2 no MS10-030. Adicionada nota sobre software afectado ao boletim MS10-031 para esclarecer que as actualizações ao Microsoft Office se aplicam a todas as suites suportadas do Microsoft Office e a outro software Microsoft Office que contenha uma versão vulnerável do VBE6.dll.

*Built at 2014-04-18T01:50:00Z-07:00*
