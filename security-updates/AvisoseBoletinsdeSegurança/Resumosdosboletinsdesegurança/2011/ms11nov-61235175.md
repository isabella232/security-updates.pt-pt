---
TOCTitle: 'MS11-NOV'
Title: Resumo dos Boletins de Segurança Microsoft de Novembro de 2011
ms:assetid: 'ms11-nov'
ms:contentKeyID: 61235175
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms11-nov(v=Security.10)'
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Novembro de 2011
==============================================================

Data de publicação: 8 de novembro de 2011

**actualizada:** 1.0

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Novembro de 2011.

Com a publicação dos boletins de segurança de Novembro de 2011, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 3 de Novembro de 2011. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação Antecipada de Boletins de Segurança da Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 9 de Novembro de 2011, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o webcast de boletins de segurança de Novembro](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032487958). Depois desta data, o webcast estará disponível mediante pedido. Para obter mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

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
<th style="border:1px solid black;" >Requisito de Reínicio</th>
<th style="border:1px solid black;" >Software Afectado</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229071">MS11-083</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no TCP/IP Poderia Permitir Execução Remota de Código (2588516)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir execução remota de código se um intruso enviasse um fluxo contínuo de pacotes UDP especialmente concebidos para o efeito a uma porta fechada num sistema de destino.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Crítica</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229638">MS11-085</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Windows Mail e no Windows Meeting Space Poderia Permitir Execução Remota de Código (2620704)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir execução remota de código se um utilizador abrisse um ficheiro legítimo (como um ficheiro .eml ou .wcinv) localizado no mesmo directório de rede que um ficheiro de biblioteca de hiperligação dinâmica (DLL) especialmente concebido. Então, ao abrir o ficheiro legítimo, o Windows Mail ou o Microsoft Meeting Space poderiam tentar carregar o ficheiro DLL e executar qualquer código nele contido. Para um ataque poder ser bem sucedido, um utilizador teria de visitar uma localização não fidedigna do sistema de ficheiros remoto ou partilha WebDAV e abrir um ficheiro legítimo (como um ficheiro .eml ou .wcinv) desta localização que é então carregado por uma aplicação vulnerável.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Execução Remota de Código</td>
<td style="border:1px solid black;">Pode requerer um reinício</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229253">MS11-086</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade no Active Directory Poderia Permitir Elevação de Privilégios (2630837)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada no Active Directory, Modo de Aplicações do Active Directory (ADAM) e Serviços LDS do Active Directory (AD LDS). A vulnerabilidade poderia permitir a elevação de privilégios se o Active Directory estiver configurado para utilizar LDAP através de SSL (LDAPS) e se um intruso adquirisse um certificado revogado associado a uma conta de domínio válida e utilizasse esse certificado revogado para se autenticar no domínio Active Directory. Por predefinição, o Active Directory não está configurado para utilizar LDAP através de SSL.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Importante</a><br />
Elevação de Privilégios</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229245">MS11-084</a></td>
<td style="border:1px solid black;"><strong>Vulnerabilidade nos Controladores de Modo de Kernel do Windows Poderia Permitir Negação de Serviço (2617657)</strong><br />
<br />
Esta actualização de segurança resolve uma vulnerabilidade no Microsoft Windows, comunicada de forma privada. A vulnerabilidade poderia permitir negação de serviço se um utilizador abrisse um ficheiro de tipo de letra TrueType especialmente concebido para o efeito como um anexo de correio electrónico ou navegasse para uma localização de partilha de rede ou WebDAV contendo um ficheiro de tipo de letra TrueType especialmente concebido para o efeito. Para um ataque poder ser bem sucedido, um utilizador deve visitar a localização não fidedigna do sistema de ficheiros remotos ou partilha WebDAV contendo o ficheiro de tipo de letra TrueType especialmente concebido para o efeito ou abrir o ficheiro como um anexo de correio electrónico. Contudo, em qualquer um dos casos, o intruso não teria forma de forçar os utilizadores a executar estas acções. Em vez disso, um intruso teria de persuadir os utilizadores a fazê-lo, levando-os normalmente a clicar numa hiperligação presente numa mensagem de correio electrónico ou numa mensagem de um programa de mensagens instantâneas.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Moderada</a><br />
Negação de Serviço</td>
<td style="border:1px solid black;">Requer reinicialização</td>
<td style="border:1px solid black;">Microsoft Windows</td>
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
  
| Identificação do Boletim                                  | Título da Vulnerabilidade                                                   | ID de CVE                                                                        | Avaliação da Possibilidade de Exploração da Execução de Código para o Lançamento de Software Mais Recente    | Avaliação da Possibilidade de Exploração da Execução de Código para Lançamentos de Software Mais Antigos     | Avaliação da Possibilidade de Exploração da Negação de Serviço | Notas Principais |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|------------------|  
| [MS11-083](http://go.microsoft.com/fwlink/?linkid=229071) | Vulnerabilidade de Sobrecarga em Contador de Referência                     | [CVE-2011-2013](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2013) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração inconsistente | Permanente                                                     | (Nenhuma)        |  
| [MS11-085](http://go.microsoft.com/fwlink/?linkid=229638) | Vulnerabilidade de Carregamento de Biblioteca sem Segurança no Windows Mail | [CVE-2011-2016](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2016) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | Não aplicável                                                  | (Nenhuma)        |  
| [MS11-086](http://go.microsoft.com/fwlink/?linkid=229253) | Vulnerabilidade em que a Autenticação LDAPS é Ignorada                      | [CVE-2011-2014](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2014) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Provável código de exploração consistente   | Não aplicável                                                  | (Nenhuma)        |
  
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
</tr>
<tr>
<th colspan="7">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
Nenhum
</td>
<td style="border:1px solid black;" colspan="2">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;" colspan="2">
[Modo de Aplicações do Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=8c7c21c5-677d-4a5d-8f2b-8ca7691b6b00)  
(KB2616310)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;" colspan="2">
[Modo de Aplicações do Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=989cca2d-cce1-4f52-b50e-43152693f240)  
(KB2616310)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
Nenhum
</td>
<td style="border:1px solid black;" colspan="2">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Nenhum
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=08b27ce7-c32e-41e4-ad04-481c5eab17a7)  
(KB2601626)  
(Importante)  
[Modo de Aplicações do Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=f116824e-ea48-422d-b284-c9ffa7604bf5)  
(KB2616310)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=de5a74f2-2cc8-4677-b495-3a40fe3d6b9e)  
(KB2601626)  
(Importante)  
[Modo de Aplicações do Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=1af1b734-62c7-4e08-91c8-90b6d026da84)  
(KB2616310)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 com SP2 para sistemas baseados em Itanium
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;">
Não aplicável
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=6168bc67-3d59-450f-bd8a-02d61dabe16b)  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
<td style="border:1px solid black;" colspan="2">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Nenhum
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc3fe87c-2493-431d-a904-dec9310f6042)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e08266d8-fffa-40bf-b8f6-10a65ee27524)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
[Serviços LDS do Active Directory (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=2bd602cf-ae0d-4790-a5d0-6133fd7d01a0)  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=042c1a8f-834d-4eed-8a59-9e030ccc6d39)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4f2365ed-d50e-44d9-b859-1ec54d3b4d38)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
[Serviços LDS do Active Directory (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=783521ad-5c50-4194-a582-4e5a1c9999e7)  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
<td style="border:1px solid black;" colspan="2">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Nenhum
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas de 32 bits Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79382bf2-d2cb-42ea-92dc-64f949353521)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas de 32 bits Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f82dc413-668c-4ca8-a8c8-db74f05346bc)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory e Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b5688923-3914-4f6c-8bc9-036fb4870cc6)\*  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71ff3a89-d7ad-4dda-9e59-fab54b21bd5d)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06ad5637-56a1-4478-aaa0-063e877503c9)\*\*  
(Moderada)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory e Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=51f47181-08f6-4de1-80e5-253355675965)\*  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 para sistemas baseados em Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1c0cb05-c284-49b1-ae4f-92813fdf520f)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 para sistemas baseados em Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2de5de74-e643-4045-9c22-ff95b0dbcafc)  
(Moderada)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
</tr>
<tr>
<th colspan="7">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
[**Baixa**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4ddb4c2a-bada-49b0-ad78-e07e7e11ced7)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2307fa93-8e45-4841-a5a9-7e89960712f9)  
(Baixo)
</td>
<td style="border:1px solid black;" colspan="2">
[Serviços LDS do Active Directory (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b06f9f55-e3b2-4705-83d0-1b9f5de9d378)  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows 7 para sistemas de 32 bits e Windows 7 para sistemas de 32 bits Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=156c1bd9-55bc-482c-874b-61998d1ef153)  
(Moderada)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=05eef5d7-acf6-46e4-abfc-dc83f0a7cae5)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=62603d18-1b21-400c-8eba-202193182960)  
(Baixo)
</td>
<td style="border:1px solid black;" colspan="2">
[Serviços LDS do Active Directory (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=790f1d99-96a5-438d-b433-895b692912ce)  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows 7 para sistemas baseados em x64 e Windows 7 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5c7db930-5495-43f0-928c-d586ac9e80d0)  
(Moderada)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identificador do Boletim**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
[**Baixa**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Importante**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Moderada**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3f9f74a6-e984-4aab-837c-ef7286e7305f)\*  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c9cf6a22-f9ab-427a-9b16-33c60baaabb5)\*\*  
(Baixo)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory e Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=cc1e99af-fc67-400b-a82c-171f8c4d1ac9)\*  
(KB2601626)  
(Importante)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows Server 2008 R2 para sistemas baseados em x64 e Windows Server 2008 R2 para sistemas baseados em x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5d810dae-5c52-4155-b5c2-163d27be6e78)\*\*\*  
(Moderada)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b20bfcbd-a515-4074-b56e-b82539fe5bad)  
(Crítica)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=012777f5-51f2-4944-91af-a9c79b8081a1)  
(Baixo)
</td>
<td style="border:1px solid black;" colspan="2">
Não aplicável
</td>
<td style="border:1px solid black;" colspan="2">
[Windows Server 2008 R2 para sistemas baseados em Itanium e Windows Server 2008 R2 para sistemas baseados em Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=395819e2-1028-44b7-ace4-ca754b1a7543)  
(Moderada)
</td>
</tr>
</table>
 
**Notas** **para o Windows Server 2008 e Windows Server 2008 R2**

**\*Instalação Server Core afectada.** Esta actualização aplica-se, com a mesma classificação de gravidade, a edições suportadas do Windows Server 2008 ou Windows Server 2008 R2, conforme indicado, quer a instalação tenha sido efectuada ou não utilizando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 e Windows Server 2008 R2 como indicado, se estes tiverem sido instalados usando a opção de instalação Server Core. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*Instalação Server Core não afectada.** A vulnerabilidade resolvida por esta actualização não afecta as edições suportadas do Windows Server 2008 ou Windows Server 2008 R2 como indicado, quando instaladas utilizando a opção de instalação Server Core, embora possam estar presentes no sistema ficheiros afectados por esta vulnerabilidade. Contudo, os utilizadores com ficheiros afectados continuarão a receber esta actualização porque os ficheiros actualizados são mais recentes (com números de versão superiores) do que os ficheiros actualmente no seu sistema. Para obter mais informações sobre esta opção de instalação, consulte os artigos TechNet sobre [Gestão de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) e [Manutenção de uma Instalação Server Core](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008 e Windows Server 2008 R2. Consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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

-   Will Dorman, da [CERT/CC](http://www.cert.org/), por fornecer informações sobre uma questão descrita no boletim MS11-084
-   Ivan Sanchez, da EvilCode, por fornecer informações sobre uma questão descrita no boletim MS11-085
-   Xavier Lassoie e Sébastien Godard, da Autosécurité, por fornecerem informações sobre uma questão descrita no boletim MS11-086

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico através do [Suporte de Segurança](http://go.microsoft.com/fwlink/?linkid=21131) ou da linha 1-866-PCSAFETY (1-866-727-2338). As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas. Para obter mais informações sobre as opções de suporte disponíveis, consulte a [Ajuda e Suporte da Microsoft](http://support.microsoft.com/).
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para obter mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (8 de Novembro de 2011): Publicação do Resumo dos Boletins.

*Built at 2014-04-18T01:50:00Z-07:00*
