---
TOCTitle: 'MS07-NOV'
Title: Resumo dos Boletins de Segurança Microsoft de Novembro 2007
ms:assetid: 'ms07-nov'
ms:contentKeyID: 61235142
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms07-nov(v=Security.10)'
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Novembro 2007
===========================================================

Data de publicação: 13 de novembro de 2007

**actualizada:** 1.0

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Novembro de 2007.

Com a publicação dos boletins de Novembro de 2007, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 8 de Novembro de 2007. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação antecipada de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 14 de Novembro de 2007, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o webcast de boletins de segurança de Novembro](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344694&eventcategory=4&culture=en-us&countrycode=us). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

A Microsoft também fornece informações para ajudar os clientes a dar prioridade às actualizações de segurança mensais com quaisquer actualizações de elevada prioridade não relacionadas com segurança que sejam lançadas no mesmo dia que as actualizações de segurança mensais. Consulte a secção: **Outras informações**.

### Informação do Boletim

#### Resumos Executivos

Os boletins de segurança deste mês são os seguintes, por ordem de gravidade:

Críticas (1)
------------

<span></span>
| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-061                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade de processamento de URI no Windows poderia permitir Execução Remota de Código (943460)**](http://go.microsoft.com/fwlink/?linkid=103190)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Resumo Executivo**                  | Esta actualização resolve uma vulnerabilidade comunicada publicamente. Existe uma vulnerabilidade de execução remota de código na forma como a Shell do Windows processa URIs especialmente concebidos para o efeito, que lhe são transmitidos. Se a Shell do Windows não fizer uma validação suficiente destes URIs, um intruso poderá explorar esta vulnerabilidade e executar código arbitrário. A Microsoft apenas identificou formas de explorar esta vulnerabilidade em sistemas que utilizam o Internet Explorer 7. Contudo, a vulnerabilidade existe num ficheiro do Windows, Shell32.dll, que está incluído em todas as edições suportadas do Windows XP e Windows Server 2003. |
| **Classificação de Gravidade Máxima** | [Crítica](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Software Afectado**                 | **Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

Importantes (1)
---------------

<span></span>
| Identificador do Boletim              | Boletim de Segurança Microsoft MS07-062                                                                                                                                                                                                                                                                                                                                                              |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade no DNS poderia permitir Ocultação de Conteúdos (941672)**](http://go.microsoft.com/fwlink/?linkid=99391)                                                                                                                                                                                                                                                                          |
| **Resumo Executivo**                  | Esta actualização de segurança importante resolve uma vulnerabilidade comunicada de forma privada. Esta vulnerabilidade de ocultação existe nos conteúdos nos servidores DNS do Windows e poderia permitir que um intruso enviasse respostas especialmente concebidas para o efeito a pedidos de DNS, ocultando conteúdos ou redireccionando tráfego de Internet a partir de localizações legítimas. |
| **Classificação de Gravidade Máxima** | [Importante](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                           |
| **Impacto da Vulnerabilidade**        | Ocultação                                                                                                                                                                                                                                                                                                                                                                                            |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer o reinício, excepto em algumas situações.                                                                                                                                                                                                                      |
| **Software Afectado**                 | **Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                   |

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
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS07-061**](http://go.microsoft.com/fwlink/?linkid=103190)
</td>
<td style="border:1px solid black;">
[**MS07-062**](http://go.microsoft.com/fwlink/?linkid=99391)
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
</tr>
<tr>
<th colspan="3">
Sistema operativo Windows
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Server Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=c80fcd9b-d0f8-44db-96fc-bf2ead054ff4)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=8ba1c2f9-1bde-4e97-b327-21259c5e5104)
</td>
<td style="border:1px solid black;">
** **
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=4ef7fdd7-8887-4c64-a70c-c6ae734d7c5f)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=4ef7fdd7-8887-4c64-a70c-c6ae734d7c5f)
</td>
<td style="border:1px solid black;">
** **
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=e5d8a866-2c1f-4035-8325-c1be61a75c3b)
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=ed8e2cb4-bcd9-40fc-9ad6-46b364d0656d)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=e5d8a866-2c1f-4035-8325-c1be61a75c3b)
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=ed8e2cb4-bcd9-40fc-9ad6-46b364d0656d)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=bf26da08-15b8-4d65-ba12-4cc74c7a1326)
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=d1323e14-ffa7-4d03-a2a7-9240c192a75e)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=bf26da08-15b8-4d65-ba12-4cc74c7a1326)
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=d1323e14-ffa7-4d03-a2a7-9240c192a75e)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 com SP1 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=1c055f11-3273-4a4c-a33f-bf61ac9ec4c5)
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=f3ad67de-85ad-452d-a1e0-0af3faf969d6)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Crítica](http://www.microsoft.com/downloads/details.aspx?familyid=1c055f11-3273-4a4c-a33f-bf61ac9ec4c5)
</td>
<td style="border:1px solid black;">
[Importante](http://www.microsoft.com/downloads/details.aspx?familyid=f3ad67de-85ad-452d-a1e0-0af3faf969d6)
</td>
</tr>
</table>
 

Orientações e ferramentas de detecção e implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para mais informações, visite o [Centro de Gestão de Actualizações TechNet](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem em “Actualizações de segurança recentes”.

As actualizações de segurança estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt), no [Windows Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt) e no [Office Update](http://office.microsoft.com/pt-pt/downloads/default.aspx). As actualizações de segurança estão também disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".

Finalmente, as actualizações de segurança podem ser transferidas a partir do [Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). O Catálogo do Microsoft Update permite pesquisar conteúdos disponibilizados através do Windows Update e do Microsoft Update, incluindo actualizações de segurança, controladores e service packs. Utilizando o número do boletim de segurança para pesquisar (por exemplo, "MS07-036"), pode adicionar todas as actualizações aplicáveis ao seu cesto (incluindo diferentes idiomas para uma actualização) e transferi-las para uma pasta à sua escolha. Para mais informação sobre o Catálogo do Microsoft Update, consulte as [Perguntas mais frequentes sobre o Catálogo do Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Orientações de detecção e implementação**

A Microsoft forneceu orientações sobre a detecção e implementação das actualizações de segurança deste mês. Estas orientações também auxiliarão os profissionais de informática a compreenderem de que forma podem usar diferentes ferramentas de suporte à implementação de actualizações de segurança, tais como o Windows Update, o Microsoft Update, o Office Update, o Microsoft Baseline Security Analyzer (MBSA), a Office Detection Tool, o Microsoft Systems Management Server (SMS) e a Extended Security Update Inventory Tool (ESUIT). Para obter mais informações, consulte o [Artigo 910723 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/910723/pt).

**Microsoft Baseline Security Analyzer**

O Microsoft Baseline Security Analyzer (MBSA) permite aos administradores procurar actualizações de segurança em falta e comuns erros de configuração de segurança em sistemas locais e remotos. Para obter mais informações acerca do MBSA, visite o Web site do [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Nota** A partir de 9 de Outubro de 2007, o ficheiro MSSecure.XML utilizado pelo MBSA 1.2.1 deixará de ser actualizado. Depois desta data, não serão adicionadas novas actualizações de segurança ao ficheiro MSSecure.XML utilizado pelo MBSA 1.2.1 e não serão lançadas novas versões da ferramenta Enterprise Scan Tool. Isto não afecta a Security Update Inventory Tool (SUIT) ou a Extended Security Update Inventory Tool (ESUIT) para SMS 2.0 e SMS 2003. Para obter mais informações, visite [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Ao utilizar os Windows Server Update Services (WSUS), os administradores podem rápida e fiavelmente implementar as actualizações críticas mais recentes e as actualizações de segurança para os sistemas operativos Windows 2000 e posteriores, Office XP e posteriores, Exchange Server 2003 e SQL Server 2000 para Windows 2000 e sistemas operativos posteriores.

Para mais informações sobre como implementar esta actualização de segurança usando os Windows Server Update Services, visite o [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

O Microsoft Systems Management Server (SMS) fornece uma solução empresarial altamente configurável para gerir actualizações. O SMS permite aos administradores identificarem sistemas baseados no Windows que necessitem de actualizações de segurança e executar a implementação controlada dessas actualizações em toda a empresa, com um mínimo de incómodo para os utilizadores finais. Para mais informações sobre como os administradores podem utilizar o SMS 2003 para implementar actualizações de segurança, visite [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Os utilizadores do SMS 2.0 também podem utilizar o [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) para ajudar na implementação das actualizações de segurança. Para informações sobre o SMS, visite [Microsoft Systems Management Server](http://www.microsoft.com/portugal/smserver/default.mspx).

**Nota** O SMS utiliza as ferramentas Microsoft Baseline Security Analyzer e Microsoft Office Detection Tool para fornecer um suporte abrangente na detecção e implementação de actualizações dos boletins de segurança. Algumas actualizações de software poderão não ser detectadas por estas ferramentas. Nestes casos, os administradores podem utilizar as capacidades de inventário do SMS para fornecer actualizações a sistemas específicos. Para mais informações sobre este procedimento, veja o artigo sobre como [Implementar actualizações de software utilizando a funcionalidade SMS Software Distribution](http://go.microsoft.com/fwlink/?linkid=33341). Algumas actualizações de segurança requerem direitos administrativos após o reinício do sistema. Os administradores podem utilizar a ferramenta Elevated Rights Deployment Tool (disponível no [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) e no [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)) para instalar estas actualizações.

### Outras informações

#### Ferramenta de Remoção de Software Malicioso Windows

A Microsoft publicou uma versão actualizada da Ferramenta de Remoção de Software Malicioso para o Microsoft Windows no Windows Update, no Microsoft Update, no Windows Server Update Services e no Centro de Transferências.

#### Actualizações não relacionadas com segurança, de elevada prioridade, no MU, WU e WSUS

Para este mês:

-   A Microsoft lançou três actualizações **não relacionadas com segurança**, de elevada prioridade, no Microsoft Update (MU) e no Windows Server Update Services (WSUS).
-   A Microsoft não lançou qualquer actualização de elevada prioridade, **não relacionada com segurança**, para o Windows no Windows Update (WU).

Note que esta informação refere-se **apenas** a actualizações **não relacionadas com segurança**, de elevada prioridade, no Microsoft Update, Windows Update e Windows Server Update Services, lançadas no mesmo dia que o resumo de boletins de segurança. Note que **não** é disponibilizada informação sobre actualizações **não relacionadas com segurança** publicadas noutros dias.

#### Estratégias e comunidades de segurança

**Estratégias de Gestão de Actualizações:**

As [orientações de segurança para Patch Management](http://go.microsoft.com/fwlink/?linkid=21168) fornecem informações adicionais referentes a recomendações de melhores práticas da Microsoft para a aplicação de actualizações de segurança.

**Obter Outras Actualizações de Segurança**

Estão disponíveis actualizações para outros problemas de segurança nas seguintes localizações:

-   As actualizações de segurança estão disponíveis no [Centro de Transferências da Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Pode encontrá-las mais facilmente através de uma procura pelas palavras "security update".
-   As actualizações para plataformas de consumidor estão disponíveis no [Microsoft Update](http://update.microsoft.com/microsoftupdate/v6/default.aspx?ln=pt-pt).
-   Pode obter as actualizações de segurança oferecidas no Windows Update este mês no ficheiro de imagem de CD em formato ISO com as informações de segurança e críticas no Centro de Transferências. Para mais informações, consulte o [Artigo 913086 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/913086).

**IT Pro Security Community**

Aprenda a melhorar a segurança, optimize a sua infra-estrutura informática e participe em tópicos de segurança juntamente com outros profissionais de informática no Web site [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Agradecimentos

A Microsoft [agradece](http://go.microsoft.com/fwlink/?linkid=21127) às seguintes entidades por trabalharem connosco para proteger os clientes:

-   Jesper Johansson, , por trabalhar connosco numa questão descrita no boletim MS07-061
-   Carsten H. Eiram, da [Secunia](http://corporate.secunia.com/), por trabalhar connosco numa questão descrita no boletim MS07-061
-   Aviv Raff, da [Finjan](http://www.finjan.com/), por trabalhar connosco numa questão descrita no boletim MS07-061
-   Petko Petkov, da [GNUCITIZEN](http://www.gnucitizen.org/), por trabalhar connosco numa questão descrita no boletim MS07-061
-   Alla Berzroutchko, da [Scanit](http://www.scanit.be/), por fornecer informações sobre uma questão descrita no boletim MS07-062
-   Amit Klein,da [Trusteer](http://www.trusteer.com/), por fornecer informações sobre uma questão descrita no boletim MS07-062

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico a partir do Web site de [Suporte Técnico da Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) em 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas.
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (13 de Novembro de 2007): Publicação do Resumo dos Boletins.

*Built at 2014-04-18T01:50:00Z-07:00*
