---
TOCTitle: 'MS07-JUL'
Title: Resumo dos Boletins de Segurança Microsoft de Julho 2007
ms:assetid: 'ms07-jul'
ms:contentKeyID: 61235139
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms07-jul(v=Security.10)'
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Julho 2007
========================================================

Data de publicação: 10 de julho de 2007 | Updated: 25 de março de 2008

**actualizada:** 2.0

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Julho de 2007.

Com a publicação dos boletins de Julho de 2007, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 5 de Julho de 2007. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação antecipada de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 11 de Julho de 2007, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o Webcast de boletins de segurança de Julho](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032343783&eventcategory=4&culture=en-us&countrycode=us). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

A Microsoft também fornece informações para ajudar os clientes a dar prioridade às actualizações de segurança mensais com quaisquer actualizações de elevada prioridade não relacionadas com segurança que sejam lançadas no mesmo dia que as actualizações de segurança mensais. Consulte a secção: **Outras informações**.

### Informação do Boletim

#### Resumos Executivos

Os boletins de segurança deste mês são os seguintes, por ordem de gravidade:

Críticas (3)
------------

<span></span>
| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-036                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidades no Microsoft Excel poderiam permitir Execução Remota de Código (936542)**](http://go.microsoft.com/fwlink/?linkid=93447)                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Resumo Executivo**                  | Esta actualização crítica resolve uma vulnerabilidade divulgada publicamente e duas vulnerabilidades comunicadas de forma privada, além de outras questões de segurança identificadas durante a investigação. Estas vulnerabilidades poderiam permitir a execução remota de código se um utilizador abrisse um ficheiro Excel especialmente concebido para o efeito. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. |
| **Classificação de Gravidade Máxima** | [Crítica](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. Esta actualização não requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Software Afectado**                 | **Office, Excel**. Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-039                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade no Active Directory do Windows poderia permitir a Execução Remota de Código (926122)**](http://go.microsoft.com/fwlink/?linkid=93365)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Resumo Executivo**                  | Esta actualização de segurança crítica resolve uma vulnerabilidade comunicada de forma privada em implementações do Active Directory no Windows 2000 Server e Windows Server 2003 que poderia permitir uma execução remota de código ou uma condição de negação de serviço. As tentativas de exploração desta vulnerabilidade iriam muito provavelmente resultar numa condição de negação de serviço. No entanto, poderia ser possível a execução remota de código. No Windows Server 2003, um intruso teria de ter credenciais de início de sessão válidas para explorar esta vulnerabilidade. Um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas, ver, alterar ou eliminar dados, ou ainda criar novas contas. |
| **Classificação de Gravidade Máxima** | [Crítica](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Software Afectado**                 | **Windows**. Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-040                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidades no .NET Framework poderiam permitir Execução Remota de Código (931212)**](http://go.microsoft.com/fwlink/?linkid=91233)                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Resumo Executivo**                  | Esta actualização resolve três vulnerabilidades comunicadas de forma privada. Duas dessas vulnerabilidades poderiam permitir a execução remota de código em sistemas clientes com o .NET Framework instalado e uma das vulnerabilidades poderia permitir a divulgação de informações em servidores Web a executar o ASP.NET. Em todas as situações de execução remota de código, os utilizadores cujas contas estão configuradas com menos direitos de utilizador no sistema seriam menos afectados do que os utilizadores que operam com direitos de utilizador administrativos. |
| **Classificação de Gravidade Máxima** | [Crítica](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Software Afectado**                 | **.NET Framework**. Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

Importante (2)
--------------

<span></span>

| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-037                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade no Microsoft Office Publisher poderia permitir Execução Remota de Código (936548)**](http://go.microsoft.com/fwlink/?linkid=93448)                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Resumo Executivo**                  | Esta actualização de segurança importante corrige uma vulnerabilidade divulgada publicamente. Esta vulnerabilidade poderia permitir a execução remota de código se um utilizador visualizasse um ficheiro Microsoft Office Publisher especialmente concebido para o efeito. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. É necessária interacção do utilizador para explorar esta vulnerabilidade. |
| **Classificação de Gravidade Máxima** | [Importante](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização não requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Software Afectado**                 | **Office, Publisher**. Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                  |

| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-041                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade no Microsoft Internet Information Services poderia permitir Execução Remota de Código (939373)**](http://go.microsoft.com/fwlink/?linkid=93706)                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Resumo Executivo**                  | Esta actualização de segurança importante resolve uma vulnerabilidade comunicada de forma privada. Esta vulnerabilidade poderia permitir uma execução remota de código se um intruso enviasse pedidos URL especialmente concebidos para o efeito para uma página Web alojada pelo Internet Information Services (IIS) 5.1 no Windows XP Professional Service Pack 2. O IIS 5.1 não faz parte da instalação predefinida do Windows XP Professional Service Pack 2. Um intruso que conseguisse explorar esta vulnerabilidade com sucesso poderia assumir o controlo total de um sistema afectado. |
| **Classificação de Gravidade Máxima** | [Importante](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Software Afectado**                 | **Windows XP Professional**. Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

Moderadas (1)
-------------

<span></span>
| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-038                                                                                                                                                                                                                                                      |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade na Firewall do Windows Vista poderia permitir a Divulgação de Informações (935807)**](http://go.microsoft.com/fwlink/?linkid=91033)                                                                                                                                       |
| **Resumo Executivo**                  | Esta actualização de segurança moderada resolve uma vulnerabilidade comunicada de forma privada. Esta vulnerabilidade poderia permitir que a entrada de tráfego de rede não solicitado acedesse a uma interface de rede. Um intruso poderia recolher informações sobre o anfitrião afectado. |
| **Classificação de Gravidade Máxima** | [Moderada](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                     |
| **Impacto da Vulnerabilidade**        | Divulgação de Informações                                                                                                                                                                                                                                                                    |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                           |
| **Software Afectado**                 | **Windows** **Vista**. Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                 |

Localizações do Software Afectado e das Transferências
------------------------------------------------------

<span></span>
**Como utilizar esta tabela?**

Utilize esta tabela para saber mais sobre as actualizações de segurança que poderá ter de instalar. Deverá rever cada programa ou componente de software listado, para ver se é necessário instalar alguma actualizações de segurança. Se um programa ou componente de software estiver listado, o impacto da vulnerabilidade é listado e é fornecida uma hiperligação para a actualização de software disponível.

**Nota** Poderá ter que instalar diversas actualizações de segurança para a mesma vulnerabilidade. Reveja toda a coluna para cada identificador de boletim listado, para verificar quais as actualizações que tem que instalar, com base nos programas ou componentes que tem instalados no seu sistema.

**Localizações do Software Afectado e das Transferências**

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Detalhes        
</th>
<th style="border:1px solid black;" >
Detalhes        
</th>
<th style="border:1px solid black;" >
Detalhes        
</th>
<th style="border:1px solid black;" >
Detalhes        
</th>
<th style="border:1px solid black;" >
Detalhes        
</th>
<th style="border:1px solid black;" >
Detalhes        
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS07-036**](http://go.microsoft.com/fwlink/?linkid=93447)
</td>
<td style="border:1px solid black;">
[**MS07-037**](http://go.microsoft.com/fwlink/?linkid=93448)
</td>
<td style="border:1px solid black;">
[**MS07-038**](http://go.microsoft.com/fwlink/?linkid=91033)
</td>
<td style="border:1px solid black;">
[**MS07-039**](http://go.microsoft.com/fwlink/?linkid=93365)
</td>
<td style="border:1px solid black;">
[**MS07-040**](http://go.microsoft.com/fwlink/?linkid=91233)
</td>
<td style="border:1px solid black;">
[**MS07-041**](http://go.microsoft.com/fwlink/?linkid=93706)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Classificação de Gravidade Máxima**
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
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Crítica**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="7">
Software Windows Afectado
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 2000 Server Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=812e62c5-6e19-4b3b-8a10-861b871e1b41)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=fccbfe90-f838-47df-8310-352e2fb47132)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 com SP1 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Moderada](http://www.microsoft.com/downloads/details.aspx?familyid=e9b64746-6afa-4a30-833d-e058e000c821)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Moderada](http://www.microsoft.com/downloads/details.aspx?familyid=0df5d190-3ad7-42d5-8629-43c47ec450cb)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7">
Componentes Afectados do Sistema Operativo Windows
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB928367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=91d7afe4-069b-4ce8-976e-9a01345a8603)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB930494)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=829a2c5b-11ec-4ed7-91ab-6961034147bc)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB928366)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=281fb2cd-c715-4f05-a01f-0455d2d9ebfb)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB933854)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=2495e656-1e0a-4b83-90da-821e68067a71)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB929729)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=7eea368d-7b82-4583-8537-30351718a4e9)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB928365)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=ba3ceb78-8e1b-4c38-adfd-e8bc95ae548d)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB929916)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=cbc9f3cf-c3c3-45c4-82e3-e11398bc2cd2)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7">
Software Office Afectado
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Excel 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=83d94d8e-dda6-4d74-b40d-476c2f0a3af4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Excel 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=9d93c0ce-5124-4234-ba84-3c27005e010f)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Excel 2003 Viewer
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=11f42977-8828-494a-a183-d1aba827b708)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Excel 2007
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=9ab28283-0320-4527-b033-5e80ef32cd34)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Pack de Compatibilidade para Office para formatos de ficheiros Word, Excel e PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=e592ae5b-09ac-4f5b-b457-a54c9850ad4a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Publisher 2007
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=25d272e7-f2dd-4342-92be-7ebc2e770b44)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 
**Notas**

**<sup>[1]</sup>** Está disponível uma actualização de segurança para este sistema operativo. Consulte o software ou componente afectado na tabela e o respectivo boletim de segurança para mais informações.** **

** **

Orientações e ferramentas de detecção e implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para mais informações, visite o [Centro de Gestão de Actualizações TechNet](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem em “Actualizações de segurança recentes”.

As actualizações de segurança estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt), no [Windows Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt) e no [Office Update](http://office.microsoft.com/pt-pt/downloads/default.aspx). As actualizações de segurança estão também disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security\_patch". Finalmente, as actualizações de segurança podem ser transferidas a partir do Catálogo do Windows Update. Para mais informações sobre o Catálogo do Windows Update, consulte o [Artigo 323166 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/323166/pt).

**Orientações de detecção e implementação**

A Microsoft forneceu orientações sobre a detecção e implementação das actualizações de segurança deste mês. Estas orientações também auxiliarão os profissionais de informática a compreenderem de que forma podem usar diferentes ferramentas de suporte à implementação de actualizações de segurança, tais como o Windows Update, o Microsoft Update, o Office Update, o Microsoft Baseline Security Analyzer (MBSA), a Office Detection Tool, o Microsoft Systems Management Server (SMS), a Extended Security Update Inventory Tool e a Enterprise Update Scan Tool (EST). Para obter mais informações, consulte o [Artigo 910723 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/910723/pt).

**Microsoft Baseline Security Analyzer e** **Enterprise** **Update Scan Tool**

O Microsoft Baseline Security Analyzer (MBSA) permite aos administradores procurar actualizações de segurança em falta e comuns erros de configuração de segurança em sistemas locais e remotos. Para obter mais informações acerca do MBSA, visite o Web site do [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

Quando a ferramenta MBSA 1.2.1 não consegue suportar a detecção de uma actualização de segurança específica, a Microsoft lança uma versão da ferramenta Enterprise Update Scan Tool (EST) para essa actualização de segurança específica. Para mais informações sobre a ferramenta EST, visite [Enterprise Update Scan Tool](http://support.microsoft.com/default.aspx?id=894193).

**Nota** A partir de 9 de Outubro de 2007, o ficheiro MSSecure.XML utilizado pelo MBSA 1.2.1 deixará de ser actualizado. Depois desta data, não serão adicionadas novas actualizações de segurança ao ficheiro MSSecure.XML utilizado pelo MBSA 1.2.1 e não serão lançadas novas versões da ferramenta Enterprise Scan Tool. Para obter mais informações, visite [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Software Update Services**

Utilizando os Microsoft Software Update Services (SUS) os administradores podem implementar rápida e eficazmente as mais recentes actualizações críticas e actualizações de segurança em servidores baseados no Windows 2000 e no Windows Server 2003, bem como em sistemas de computadores de secretária que executem o Windows 2000 Professional ou o Windows XP Professional.

Para mais informações sobre como implementar esta actualização de segurança com o Software Update Services, visite o [Software Update Services](http://go.microsoft.com/fwlink/?linkid=21133).

**Windows Server Update Services**

Ao utilizar os Windows Server Update Services (WSUS), os administradores podem rápida e fiavelmente implementar as actualizações críticas mais recentes e as actualizações de segurança para os sistemas operativos Windows 2000 e posteriores, Office XP e posteriores, Exchange Server 2003 e SQL Server 2000 para Windows 2000 e sistemas operativos posteriores.

Para mais informações sobre como implementar esta actualização de segurança usando os Windows Server Update Services, visite o [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

O Microsoft Systems Management Server (SMS) fornece uma solução empresarial altamente configurável para gerir actualizações. O SMS permite aos administradores identificarem sistemas baseados no Windows que necessitem de actualizações de segurança e executar a implementação controlada dessas actualizações em toda a empresa, com um mínimo de incómodo para os utilizadores finais. Para mais informações sobre como os administradores podem utilizar o SMS 2003 para implementar actualizações de segurança, visite [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Os utilizadores do SMS 2.0 também podem utilizar o [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) para ajudar na implementação das actualizações de segurança. Para informações sobre o SMS, visite [Microsoft Systems Management Server](http://www.microsoft.com/portugal/smserver/default.mspx).

**Nota** O SMS utiliza as ferramentas Microsoft Baseline Security Analyzer e Microsoft Office Detection Tool para fornecer um suporte abrangente na detecção e implementação de actualizações dos boletins de segurança. Algumas actualizações de software poderão não ser detectadas por estas ferramentas. Nestes casos, os administradores podem utilizar as capacidades de inventário do SMS para fornecer actualizações a sistemas específicos. Para mais informações sobre este procedimento, veja o artigo sobre como [Implementar actualizações de software utilizando a funcionalidade SMS Software Distribution](http://go.microsoft.com/fwlink/?linkid=33341). Algumas actualizações de segurança requerem direitos administrativos após o reinício do sistema. Os administradores podem utilizar a ferramenta Elevated Rights Deployment Tool (disponível no [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) e no [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)) para instalar estas actualizações.

### Outras informações

#### Ferramenta de Remoção de Software Malicioso Windows

A Microsoft publicou uma versão actualizada da Ferramenta de Remoção de Software Malicioso para o Microsoft Windows no Windows Update, no Microsoft Update, no Windows Server Update Services e no Centro de Transferências.

Note que esta ferramenta **não** é distribuída pelos Software Update Services (SUS).

#### Actualizações não relacionadas com segurança, de elevada prioridade, no MU, WU, WSUS e SUS

Para este mês:

-   A Microsoft lançou quatro actualizações **não relacionadas com segurança**, de elevada prioridade, no Microsoft Update (MU) e no Windows Server Update Services (WSUS).
-   A Microsoft lançou uma actualização **não relacionada com segurança**, de elevada prioridade para o Windows, no Windows Update (WU) e Software Update Services (SUS).

Note que esta informação refere-se **apenas** a actualizações **não relacionadas com segurança**, de elevada prioridade no Microsoft Update, Windows Update, Windows Server Update Services e Software Update Services, lançados no mesmo dia que o resumo de boletins de segurança. Note que **não** é disponibilizada informação sobre actualizações **não relacionadas com segurança** publicadas noutros dias.

#### Estratégias e comunidades de segurança

**Estratégias de Gestão de Actualizações**

As [orientações de segurança para Patch Management](http://go.microsoft.com/fwlink/?linkid=21168) fornecem informações adicionais referentes a recomendações de melhores práticas da Microsoft para a aplicação de actualizações de segurança.

**Obter Outras Actualizações de Segurança**

Estão disponíveis actualizações para outros problemas de segurança nas seguintes localizações:

-   As actualizações de segurança estão disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras-chave "security\_patch".
-   As actualizações para plataformas de consumidor estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt).
-   Pode obter as actualizações de segurança oferecidas no Windows Update este mês no ficheiro de imagem de CD em formato ISO com as informações de segurança e críticas no Centro de Transferências. Para mais informações, consulte o [Artigo 913086 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/913086).

**IT Pro Security Community**

Aprenda a melhorar a segurança, optimize a sua infra-estrutura informática e participe em tópicos de segurança juntamente com outros profissionais de informática no Web site [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Agradecimentos

A Microsoft [agradece](http://go.microsoft.com/fwlink/?linkid=21127) às seguintes entidades por trabalharem connosco para proteger os clientes:

-   Dinis Cruz, da [OWASP](http://www.owasp.org/), por fornecer informações sobre uma questão descrita no boletim [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Paul Craig, da [Security Assessment](http://www.smsiinc.com/), por fornecer informações sobre uma questão descrita no boletim [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Jeroen Frijters, da [Sumatra](http://www.sumatra.nl/), por fornecer informações sobre uma questão descrita no boletim [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   [ProCheckUp](http://www.procheckup.com/), a trabalhar com a [UK CPNI](http://www.cpni.gov.uk/), por fornecer as primeiras informações sobre uma questão descrita no boletim [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Ferruh T. Mavituna, da [Portcullis Computer Security Ltd.](http://www.portcullis-security.com/), por trabalhar com a Microsoft e fornecer informações adicionais sobre uma questão descrita no boletim [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Johannes Gumbel, da [TrueSec](http://www.truesec.com/), por trabalhar com a Microsoft e fornecer informações adicionais sobre uma questão descrita no boletim [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Peter Winter-Smith, da [NGSSoftware](http://www.nextgenss.com/), por fornecer informações sobre uma questão descrita no boletim [MS07-039](http://go.microsoft.com/fwlink/?linkid=93365).
-   Neel Mehta, da [IBM Internet Security Systems x-Force](http://xforce.iss.net/), por fornecer informações sobre uma questão descrita no boletim [MS07-039](http://go.microsoft.com/fwlink/?linkid=93365).
-   [eEye](http://www.eeye.com/), por fornecer informações sobre uma questão descrita no boletim [MS07-037](http://go.microsoft.com/fwlink/?linkid=93488).
-   Jim Hoagland e Ollie Whitehouse, da [Symantec](http://www.symantec.com/), por fornecerem informações sobre uma questão descrita no boletim [MS07-038](http://go.microsoft.com/fwlink/?linkid=91033).
-   Jonathan Afek e Adi Sharabani, da [Watchfire](http://www.watchfire.com/), por trabalharem com a Microsoft e fornecerem informações adicionais sobre uma questão descrita no boletim [MS07-041](http://go.microsoft.com/fwlink/?linkid=93706).
-   Peter Winter-Smith, da [NGSSoftware](http://www.nextgenss.com/), por trabalhar com a Microsoft e fornecer informações adicionais sobre uma questão descrita no boletim [MS07-041](http://go.microsoft.com/fwlink/?linkid=93706).

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico a partir do Web site de [Suporte Técnico da Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) em 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas.
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (10 de Julho de 2007): Publicação do Resumo dos Boletins.
-   V2.0 (25 de Março de 2008): Acrescentados o Windows Vista Service Pack 1, Windows Vista x64 Edition Service Pack 1, Windows Server 2008, Windows Server 2008 para sistemas baseados em Itanium e o Windows Server 2008 x64 Edition à tabela "Software Afectado".

*Built at 2014-04-18T01:50:00Z-07:00*
