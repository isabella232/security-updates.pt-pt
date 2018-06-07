---
TOCTitle: 'MS12-JAN'
Title: Resumo dos Boletins de Segurança Microsoft de Janeiro de 2012
ms:assetid: 'ms12-jan'
ms:contentKeyID: 61235181
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms12-jan(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Janeiro de 2012
=============================================================

Data de publicação: 10 de janeiro de 2012 | Updated: 27 de janeiro de 2012

**actualizada:** 2.1

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Janeiro de 2012.

Com a publicação dos boletins de segurança de Janeiro de 2012, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 5 de Janeiro de 2012. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 11 de Janeiro de 2012, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o webcast de boletins de segurança de Janeiro](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499498). Depois desta data, o webcast estará disponível mediante pedido. Para obter mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227487">MS12-004</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidades no Windows Media Poderiam Permitir Execução Remota de Código (2636391)</strong><br />
<br />
Esta actualização de segurança resolve duas vulnerabilidades no Microsoft Windows, comunicadas de forma privada. As vulnerabilidades poderiam permitir a execução remota de código se um utilizador abrisse um ficheiro multimédia especialmente concebido para o efeito. Um intruso que explorasse as vulnerabilidades com sucesso poderia obter os mesmos direitos que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235999">MS12-001</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Kernel do Windows Poderia Permitir que Funcionalidade de Segurança fosse Ignorada (2644615)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir que um intruso ignorasse a funcionalidade de segurança SafeSEH numa aplicação de software. Um intruso poderia então utilizar outras vulnerabilidades para utilizar o processador de excepções estruturadas para executar código arbitrário. Apenas as aplicações de software compiladas utilizando o Microsoft Visual C++ .NET 2003 podem ser utilizadas para explorar esta vulnerabilidade.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Funcionalidade de Segurança Ignorada</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229637">MS12-002</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Gestor de Objectos do Windows Poderia Permitir Execução Remota de Código (2603381)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro legítimo com um objecto compactado incorporado no mesmo directório de rede que um ficheiro executável especialmente concebido para o efeito. Um intruso que conseguisse explorar esta vulnerabilidade com êxito poderia obter os mesmos privilégios que o utilizador com sessão iniciada. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235400">MS12-003</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Windows Client/Server Run-time Subsystem Poderia Permitir Elevação de Privilégios (2646524)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows comunicada de forma privada. Esta actualização de segurança está classificada como Importante para todas as edições suportadas do Windows XP, Windows Server 2003, Windows Vista e Windows Server 2008. Todas as edições suportadas do Windows 7 e do Windows Server 2008 R2 não são afectadas pela vulnerabilidade.<br />
<br />
A vulnerabilidade poderia permitir a elevação de privilégios se um intruso iniciasse sessão num sistema afectado e executasse uma aplicação especialmente concebida para o efeito. O intruso poderia então obter controlo total sobre o sistema afectado e instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Esta vulnerabilidade só pode ser explorada em sistemas com a região do sistema definida para chinês, japonês ou coreano.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=230777">MS12-005</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Microsoft Windows Poderia Permitir Execução Remota de Código (2584146)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro do Microsoft Office especialmente concebido para o efeito contendo uma aplicação ClickOnce incorporada maliciosa. Um intruso que explorasse com sucesso esta vulnerabilidade poderia obter os mesmos privilégios que o utilizador local. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232510">MS12-006</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no SSL/TLS Poderia Permitir Divulgação de Informações (2643584)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade, divulgada publicamente, no SSL 3.0 e no TLS 1.0. Esta vulnerabilidade afecta o próprio protocolo e não é específica do sistema operativo Windows. A vulnerabilidade poderia permitir divulgação de informações se um intruso interceptasse tráfego da Web encriptado servido a partir de um sistema afectado. O TLS 1.1, o TLS 1.2 e todos os conjuntos de cifras que não utilizam o modo CBC não são afectados.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Divulgação de Informações</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227561">MS12-007</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade na</strong> <strong>AntiXSS</strong> <strong>Library Poderia Permitir Divulgação de Informações (2607664)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada na Microsoft Anti-Cross Site Scripting (AntiXSS) Library. A vulnerabilidade poderia permitir divulgação de informações se um intruso transmitisse um script mal intencionado para um Web site utilizando a função de sanitização da AntiXSS Library. As consequências da divulgação dessa informação variam mediante a natureza da própria informação. Tenha em atenção que a vulnerabilidade não permitiria que um intruso executasse código ou elevasse directamente os direitos de utilizador do intruso, mas poderia ser utilizada para produzir informações que poderiam ser usadas para comprometer ainda mais o sistema afectado. Apenas os sites que utilizam o módulo de sanitização da AntiXSS Library são afectados por esta vulnerabilidade.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Divulgação de Informações</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Software e Ferramentas de Desenvolvimento da Microsoft</td>
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
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                              | ID de CVE                                                                        | Avaliação da Possibilidade de Exploração para o Lançamento de Software Mais Recente              | Avaliação da Possibilidade de Exploração para o Lançamento de Software Mais Antigo               | Avaliação da Possibilidade de Exploração da Negação de Serviço | Notas Principais                                                                                                      |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|  
| [MS12-001](http://go.microsoft.com/fwlink/?linkid=235999) | Vulnerabilidade em que a Funcionalidade SafeSEH é Ignorada no Kernel do Windows        | [CVE-2012-0001](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0001) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | Não aplicável                                                  | Esta é uma vulnerabilidade em que uma funcionalidade de segurança é ignorada.                                         |  
| [MS12-002](http://go.microsoft.com/fwlink/?linkid=229637) | Vulnerabilidade de Início de Ficheiros Executáveis sem Segurança no Gestor de Objectos | [CVE-2012-0009](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0009) | Não afectado                                                                                     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | Não aplicável                                                  | (Nenhuma)                                                                                                             |  
| [MS12-003](http://go.microsoft.com/fwlink/?linkid=235400) | Vulnerabilidade de Elevação de Privilégios no CSRSS                                    | [CVE-2012-0005](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0005) | Não afectado                                                                                     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | Permanente                                                     | (Nenhuma)                                                                                                             |  
| [MS12-004](http://go.microsoft.com/fwlink/?linkid=227487) | Vulnerabilidade de Execução Remota de Código em Ficheiros MIDI                         | [CVE-2012-0003](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0003) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | Não aplicável                                                  | (Nenhuma)                                                                                                             |  
| [MS12-004](http://go.microsoft.com/fwlink/?linkid=227487) | Vulnerabilidade de Execução Remota de Código no Direct Show                            | [CVE-2012-0004](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0004) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | Não aplicável                                                  | (Nenhuma)                                                                                                             |  
| [MS12-005](http://go.microsoft.com/fwlink/?linkid=230777) | Vulnerabilidade de Execução de Assemblagem                                             | [CVE-2012-0013](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0013) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração   | Não aplicável                                                  | (Nenhuma)                                                                                                             |  
| [MS12-006](http://go.microsoft.com/fwlink/?linkid=232510) | Vulnerabilidade nos Protocolos SSL e TLS                                               | [CVE-2011-3389](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3389) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração | Não aplicável                                                  | Trata-se de uma vulnerabilidade ao nível da divulgação de informações, divulgada publicamente com detalhes limitados. |  
| [MS12-007](http://go.microsoft.com/fwlink/?linkid=227561) | Vulnerabilidade em que a AntiXSS Library é Ignorada                                    | [CVE-2012-0007](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0007) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Improvável código de exploração | Não aplicável                                                  | Trata-se de uma vulnerabilidade ao nível da divulgação de informações.                                                |
  
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
<th colspan="7">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=a142f7ba-4268-4453-a8eb-470213c028ac)  
(KB2598479)  
(Crítica)  
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=89b23d72-410f-4133-9c14-24eb01e5a732)  
(KB2628259)  
(Windows XP Media Center Edition 2005 Service Pack 3 apenas)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=4b168ee8-eb15-4c2c-afb0-e63d62b4a6dc)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=feaeda8c-84ee-47be-8c68-736f0e5b1fc7)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cfc38dc2-c4c7-4a44-8e5a-b98bb9bc0396)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1bcb1d1e-9261-4a36-9256-90d3df9bd4fb)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fb0360b1-254c-4ecb-a36a-807cabfec1ab)  
(KB2585542)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=0928d720-ae88-40d6-b76f-636d67da8526)  
(KB2598479)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=13d74cc6-8d8e-45ea-8cdc-c15782f6626b)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46386269-6e37-4710-bfef-cedfe60d881c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=211827f2-fe6a-4e16-a90c-0cc3b60a722d)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3956db98-88d9-49fc-be51-247b40bfc272)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c687796-4c41-4d17-b738-511d2fbfc126)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=afe6b34d-21b1-4dfa-afa6-2c5c2a678e9e)  
(KB2585542)  
(Importante)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=986f1156-0190-48c2-9f39-29cacb91f0f9)  
(KB2638806)  
(Importante)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
I**dentificador do** **Boletim**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=3c266dfb-630d-4f32-b2ca-63955279b6a9)  
(KB2598479)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=89ae6ed0-537f-421c-b755-ef28691abd88)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9cdfc0fe-8f43-4e13-8a1f-2b48ff9ff472)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b8e46267-7988-4fbe-ae94-68b6fdb2e7d9)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=39f5f8fb-ee4d-4b7a-9cd7-3d1e9c8abd8c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c39be84-1eab-4794-b3ed-e529643aca21)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2c503a5-3f15-4a77-9a05-9ea0fbaf4503)  
(KB2585542)  
(Importante)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c23e7604-d489-4836-8b54-3b2b3d6a365c)  
(KB2638806)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=8dd1c882-4ed1-4e47-a017-7d162bd94194)  
(KB2598479)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=08be569c-e9d1-4fc5-8670-ebe9da0a2072)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e5783aa-6847-404c-9b75-621fa14ebbb8)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5975b01e-139b-4b9d-a0d5-a87a279bfea1)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e27d85f8-a285-4e95-85a0-0868286cc2b9)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3cf29dfd-239e-4707-92e6-952133c1c1c2)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ad34496-40af-40cb-9f85-5d3c31543211)  
(KB2585542)  
(Importante)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f36e991-4e1a-4b8c-8cfb-e7f20d97cf0b)  
(KB2638806)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=3a9b09d6-7060-47ab-9f76-c3c5acb024e6)  
(KB2598479)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=3401ac20-3701-471f-9757-097a9402d761)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=cdf8208c-d55b-428f-bdd3-26e291dfb08d)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=26079c35-4b96-42fc-ad47-138be25a6bf0)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b69bd01d-9925-4ff1-bfeb-b4473631578c)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=623c1c7d-6902-4876-9614-1b6e1ef80831)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=56deb935-9226-49f8-b705-edb3d662d8aa)  
(KB2585542)  
(Importante)  
[Windows Server 2003 com SP2 para sistemas baseados em Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2d72cf5a-cca7-4341-b862-017e3f34a3c9)  
(KB2638806)  
(Importante)
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=99d9b9fc-ed37-4a32-a20d-6604a1b9c4ca)  
(KB2598479)  
(Crítica)  
[Windows Media Center TV Pack for Windows Vista (edições de 32 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=f345e093-336d-4464-b7f8-a14398b62ebf)<sup>[1]</sup>
(KB2628642)  
(Importante)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=4818059a-52ad-4c2e-9605-4e0f5d9da5ba)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=44eeb0a2-ae17-4971-8a7e-e25b260c582c)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73682d4b-3179-4488-8ba9-94ed68c4896b)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=038970b6-aeec-4e18-8dfe-887b260a7c87)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f9269bd6-8c4f-476e-8481-fc0de52a22e6)  
(KB2585542)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=44aa8d91-2b30-4191-8965-8aee2b860d50)  
(KB2598479)  
(Crítica)  
[Windows Media Center TV Pack for Windows Vista (edições de 64 bits)](http://www.microsoft.com/downloads/details.aspx?familyid=559d028f-9810-4c50-b65d-f567cbb15427)<sup>[1]</sup>
(KB2628642)  
(Importante)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=13cc2519-860d-4c64-b7f8-8f9c0bdaefcf)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79ceba86-59a1-4138-a5de-8df20ad81b02)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b5c33025-13d9-43d2-a415-a8a4d683a821)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=23abeb12-f2fe-43fd-9c4a-4d3d244832f8)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0403c753-d4fa-4e3d-a61b-7f816f5c352b)  
(KB2585542)  
(Importante)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=787e6285-3ba5-4aae-9d8d-e3c1eca3b35d)\*  
(KB2598479)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=92df13c1-fdf6-4602-acb2-e634a1bcd9da)\*\*  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ab87c6c-5802-4454-bce4-12501e5b816d)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbf119cf-a8ed-4266-a673-442149992f7c)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d089d9cb-382c-4e64-94c5-69b9864010b1)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2fe2f398-433f-4338-a273-813185b43ea8)\*  
(KB2585542)  
(Importante)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=9eff12b2-70a4-452b-b6bc-0d83f2edcf6c)\*  
(KB2598479)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=7ff10d7f-26a6-403a-a4b7-7aff55e2fa16)\*\*  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=726ff17e-ac90-4832-91e7-46f71ad2f868)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8e68f89-27f4-4142-94ca-58f086a98157)\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ac8a368-4298-4c1d-9cfd-924d6df563af)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f54ac30d-8e41-4df9-bd43-db6742a24d4c)\*  
(KB2585542)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=4e2edb23-7f4e-4fe4-848c-1d744e0dce9f)  
(KB2598479)  
(Crítica)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=5e0394c9-3de4-46f6-ae7f-18d5a555532e)  
(KB2631813)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ba2c3d57-1bdd-44f2-9233-86c7ea6f0ddb)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc6491e8-6c3e-43a1-bc56-16c9a2fd2749)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e08b242-2516-4cf6-b38e-35ec2b8b788d)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3979db3b-4961-4df8-84a4-1f26672b127c)  
(KB2585542)  
(Importante)
</td>
</tr>
<tr>
<th colspan="7">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=d736daf8-db6d-485f-b0cb-7f2d8c86f9a2)  
(KB2631813)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0ee22036-b7f4-40f5-8f40-a77e8faf48b2)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7422605b-7a02-4161-b7f8-92b3ccffef64)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0f433f2c-c61d-461d-af9c-0145af4b72ab)  
(KB2585542)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=21b37775-3e7b-462d-8234-7c47d52daef9)  
(KB2631813)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7444e20c-9821-4c91-9779-2728c537dd6a)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4ba46bc7-af7a-445a-84f2-b0c13674409b)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0839fec0-b6a7-4e47-9da3-2caef44a7df4)  
(KB2585542)  
(Importante)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=355c980d-ec2e-4b2d-a7d4-2e3dbd3a0dde)\*\*  
(KB2631813)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4c73a16d-e9fa-48de-9dca-a6360ce3d029)\*  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=db3a4814-a409-4def-944d-4eaa540b83b0)\*\*  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34542a5a-88df-4a07-b1ed-d4c845502cd8)\*  
(KB2585542)  
(Importante)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=d4b2389e-fd9f-47c7-9afd-4077f5632c21)  
(KB2631813)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1cc14ee8-f035-4bfc-bf38-33c6b9a2e776)  
(Importante)
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2101663a-ed3d-4850-b79a-16960ab56b45)  
(Importante)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fe661936-06e1-45d3-89f6-1093504496a7)  
(KB2585542)  
(Importante)
</td>
</tr>
</table>
 
**Notas para o Windows Server 2008 e Windows Server 2008 R2**

**\*Instalação Server Core afectada.** Esta actualização aplica-se, com a mesma classificação de gravidade, a edições suportadas do Windows Server 2008 ou Windows Server 2008 R2, conforme indicado, quer a instalação tenha sido efectuada ou não utilizando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 e Windows Server 2008 R2 como indicado, se estes tiverem sido instalados usando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Nota para o MS12-004**

<sup>[1]</sup>O Windows Media Center TV Pack para Windows Vista só está disponível em instalações do fabricante de equipamento original (OEM) das edições Home Premium e Ultimate do Windows Vista como componente opcional. Os clientes com este componente opcional instalado devem instalar todas as actualizações disponíveis para a sua edição do Windows Vista. Para manter as melhores práticas, a Microsoft recomenda a instalação das actualizações aplicáveis para o sistema operativo (KB2598479 e KB2631813) antes da instalação do Windows Media Center TV Pack (KB2628642).

#### Software e Ferramentas de Desenvolvimento da Microsoft

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Anti-Cross Site Scripting Library
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do boletim**
</td>
<td style="border:1px solid black;">
[**MS12-007**](http://go.microsoft.com/fwlink/?linkid=227561)
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
Microsoft Anti-Cross Site Scripting Library V3.x e Microsoft Anti-Cross Site Scripting Library V4.0
</td>
<td style="border:1px solid black;">
[Microsoft Anti-Cross Site Scripting Library V3.x e Microsoft Anti-Cross Site Scripting Library V4.0](http://www.microsoft.com/downloads/details.aspx?familyid=b3ef05ce-70fe-4f25-9aee-cb7a42a53d11)<sup>[1]</sup><sup>[2]</sup>
</td>
</tr>
</table>
 
**Nota para o MS12-007**

<sup>[1]</sup>Esta transferência actualiza a Microsoft Anti-Cross Site Scripting (AntiXSS) Library para uma versão mais recente da Microsoft Anti-Cross Site Scripting Library que não é afectada pela vulnerabilidade.

<sup>[2]</sup>Esta actualização está disponível apenas a partir do Centro de Transferências da Microsoft.

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

O Application Compatibility Toolkit (ACT) contém as ferramentas e documentação necessárias para avaliar e atenuar questões de compatibilidade da aplicação antes de implementar o Microsoft Windows Vista, uma Actualização do Windows, uma Actualização de Segurança da Microsoft ou uma nova versão do Windows Internet Explorer no seu ambiente.

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

-   Joshua J. Drake, da [Accuvant Labs](http://www.accuvant.com/), por fornecer informações sobre uma questão descrita no boletim MS12-001
-   Parvez Anwar, a trabalhar com a [Secunia Research](http://secunia.com/), por fornecer informações sobre uma questão descrita no boletim MS12-002
-   Kang Wu, da [Shenzhen Jowto Research Dep](http://www.jowto.com), por fornecer informações sobre uma questão descrita no boletim MS12-003
-   Shane Garrett, da [IBM Security System's X-Force Research](http://xforce.iss.net/), por fornecer informações sobre uma questão descrita no boletim MS12-004
-   Neel Mehta, da [Google Inc.](http://www.google.com/), por fornecer informações sobre uma questão descrita no boletim MS12-004
-   Yorick Koster, a trabalhar com o programa [Beyond Security's SecuriTeam Secure Disclosure](http://www.beyondsecurity.com/ssd.html), por fornecer informações sobre uma questão descrita no boletim MS12-005
-   Adi Cohen, da [IBM Rational Application Security](http://blog.watchfire.com/), por fornecer informações sobre uma questão descrita no boletim MS12-007

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY (1-866-727-2338). As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre as opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para obter mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (10 de Janeiro de 2012): Publicação do Resumo dos Boletins.
-   V2.0 (11 de Janeiro de 2012): Para o MS12-003, foi corrigida a avaliação da possibilidade de exploração para o lançamento de software mais recente no **Índice de possibilidade de exploração** para o CVE-2012-0005. O MS12-007, foi revisto para anunciar o relançamento do boletim. Consulte o boletim MS12-007 para obter mais informações.
-   V2.1 (27 de Janeiro de 2012): Para o MS12-004, foi corrigida a classificação de gravidade agregada para o pacote de actualização KB2631813 para todas as edições suportadas do Windows XP, Windows Server 2003, Windows Vista e Windows Server 2008. Consulte o boletim MS12-004 para obter mais detalhes.

*Built at 2014-04-18T01:50:00Z-07:00*
