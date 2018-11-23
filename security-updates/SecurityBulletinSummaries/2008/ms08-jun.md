---
TOCTitle: 'MS08-JUN'
Title: Resumo dos Boletins de Segurança Microsoft de Junho 2008
ms:assetid: 'ms08-jun'
ms:contentKeyID: 61235145
ms:mtpsurl: 'https://technet.microsoft.com/pt-PT/library/ms08-jun(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Resumo dos Boletins de Segurança Microsoft de Junho 2008
========================================================

Data de publicação: 10 de junho de 2008 | Updated: 1 de abril de 2009

**actualizada:** 2.1

Este resumo dos boletins apresenta uma lista dos boletins de segurança publicados em Junho de 2008.

Com a publicação dos boletins de Junho de 2008, este resumo dos boletins substitui a notificação antecipada de boletins publicada a 5 de Junho de 2008. Para mais informações sobre o serviço de boletins de notificação antecipada, consulte a [Notificação antecipada de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Para informações sobre a forma de receber notificações automáticas cada vez que a Microsoft publicar boletins de segurança, visite [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

A Microsoft fará um webcast para responder a questões dos clientes sobre estes boletins no dia 11 de Junho de 2008, às 11:00, hora do Pacífico (Estados Unidos e Canadá). [Registe-se agora para o Webcast de boletins de segurança de Junho](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357225&eventcategory=4&culture=en-us&countrycode=us). Depois desta data, o webcast estará disponível mediante pedido. Para mais informações, consulte [Webcast e resumos de boletins de segurança da Microsoft](http://technet.microsoft.com/security/bulletin/summary).

A Microsoft também fornece informações para ajudar os clientes a dar prioridade às actualizações de segurança mensais com quaisquer actualizações de elevada prioridade não relacionadas com segurança que sejam lançadas no mesmo dia que as actualizações de segurança mensais. Consulte a secção: **Outras informações**.

### Informação do Boletim

#### Resumos Executivos

Os boletins de segurança deste mês são os seguintes, por ordem de gravidade:

Críticas (3)
------------

<span></span>

| Identificador do Boletim              | Boletim de Segurança Microsoft MS08-030                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade na Pilha Bluetooth poderia permitir Execução Remota de Código (951376)**](http://go.microsoft.com/fwlink/?linkid=119619)                                                                                                                                                                                                                                                                                     |
| **Resumo Executivo**                  | Esta actualização de segurança resolve uma vulnerabilidade na pilha Bluetooth no Windows, comunicada de forma privada, que poderia permitir execução remota de código. Um intruso que conseguisse tirar partido desta vulnerabilidade poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. |
| **Classificação de Gravidade Máxima** | [Crítica](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                         |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização pode requerer um reinício.                                                                                                                                                                                                                                                                       |
| **Software Afectado**                 | **Microsoft Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                    |

| Identificador do Boletim              | Boletim de Segurança Microsoft MS08-031                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Actualização de Segurança Cumulativa para o Internet Explorer (950759)**](http://go.microsoft.com/fwlink/?linkid=116367)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Resumo Executivo**                  | Esta actualização de segurança resolve uma vulnerabilidade comunicada de forma privada e uma vulnerabilidade divulgada publicamente. A vulnerabilidade comunicada de forma privada poderia permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. A vulnerabilidade divulgada publicamente poderia permitir a divulgação de informações se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer. |
| **Classificação de Gravidade Máxima** | [Crítica](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Software Afectado**                 | **Microsoft Windows, Internet Explorer.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

| Identificador do Boletim              | Boletim de Segurança Microsoft MS08-033                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidades no DirectX poderiam permitir Execução Remota de Código (951698)**](http://go.microsoft.com/fwlink/?linkid=118655)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Resumo Executivo**                  | Esta actualização de segurança corrige duas vulnerabilidades no Microsoft DirectX, comunicadas de forma privada, que poderiam permitir execução remota de código se um utilizador abrisse um ficheiro multimédia especialmente concebido para o efeito. Um intruso que conseguisse tirar partido de qualquer uma destas vulnerabilidades poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas; ver, alterar ou eliminar dados; ou ainda criar novas contas com todos os privilégios. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. |
| **Classificação de Gravidade Máxima** | [Crítica](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização pode requerer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Software Afectado**                 | **Microsoft Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

Importante (3)
--------------

<span></span>

| Identificador do Boletim              | Boletim de Segurança Microsoft MS08-034                                                                                                                                                                                                                                                                                                                                                                              |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade no WINS poderia permitir Elevação de Privilégios (948745)**](http://go.microsoft.com/fwlink/?linkid=111957)                                                                                                                                                                                                                                                                                       |
| **Resumo Executivo**                  | Esta actualização de segurança resolve uma vulnerabilidade no Windows Internet Name Service (WINS), comunicada de forma privada, que poderia permitir elevação de privilégios. Um intruso local que conseguisse tirar partido desta vulnerabilidade poderia obter o controlo total de um sistema afectado. Um intruso poderia então instalar programas, ver, alterar ou eliminar dados, ou ainda criar novas contas. |
| **Classificação de Gravidade Máxima** | [Importante](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                           |
| **Impacto da Vulnerabilidade**        | Elevação de Privilégios                                                                                                                                                                                                                                                                                                                                                                                              |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                   |
| **Software Afectado**                 | **Microsoft Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                         |

| Identificador do Boletim              | Boletim de Segurança Microsoft MS08-035                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidade no Active Directory poderia permitir Negação de Serviço (953235)**](http://go.microsoft.com/fwlink/?linkid=111953)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Resumo Executivo**                  | Esta actualização de segurança resolve uma vulnerabilidade, comunicada de forma privada, em implementações do Active Directory no Microsoft Windows 2000 Server, Windows Server 2003 e Windows Server 2008; Active Directory Application Mode (ADAM) quando instalado no Windows XP Professional e Windows Server 2003; e Active Directory Lightweight Directory Service (AD LDS) quando instalado no Windows Server 2008. A vulnerabilidade poderia ser explorada para permitir que um intruso provocasse uma condição de negação de serviço. No Windows XP Professional, Windows Server 2003 e Windows Server 2008, um intruso teria de ter credenciais de início de sessão válidas para explorar esta vulnerabilidade. Um intruso que explorasse esta vulnerabilidade com sucesso poderia fazer com que o sistema deixasse de responder ou fosse automaticamente reiniciado. |
| **Classificação de Gravidade Máxima** | [Importante](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Impacto da Vulnerabilidade**        | Negação de Serviço                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Software Afectado**                 | **Microsoft Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

| Identificador do Boletim              | Boletim de Segurança Microsoft MS08-036                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Vulnerabilidades no Pragmatic General Multicast (PGM) poderiam permitir Negação de Serviço (950762)**](http://go.microsoft.com/fwlink/?linkid=117297)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Resumo Executivo**                  | Esta actualização de segurança resolve duas vulnerabilidades no protocolo Pragmatic General Multicast (PGM), comunicadas de forma privada, que poderiam permitir uma negação de serviço se um sistema afectado recebesse pacotes PGM mal formados. Um intruso que explorasse esta vulnerabilidade com sucesso poderia fazer com que o sistema de um utilizador deixasse de responder e tivesse de ser reiniciado para restaurar a funcionalidade. Tenha em atenção que a vulnerabilidade na negação de serviço não permitiria que um intruso executasse o código ou elevasse os seus direitos de utilizador, mas poderia fazer com que o sistema afectado deixasse de aceitar pedidos. |
| **Classificação de Gravidade Máxima** | [Importante](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Impacto da Vulnerabilidade**        | Negação de Serviço                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização requer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Software Afectado**                 | **Microsoft Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |

Moderadas (1)
-------------

<span></span>

| Identificador do Boletim              | Boletim de Segurança Microsoft MS08-032                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Título do Boletim**                 | [**Actualização de Segurança Cumulativa de Kill Bits do ActiveX (950760)**](http://go.microsoft.com/fwlink/?linkid=116368)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Resumo Executivo**                  | Esta actualização de segurança resolve uma vulnerabilidade comunicada publicamente para o Microsoft Speech API. A vulnerabilidade poderia permitir a execução remota de código se um utilizador visualizasse uma página Web especialmente concebida para o efeito utilizando o Internet Explorer e se a funcionalidade de Reconhecimento de Voz no Windows estivesse activada. Os utilizadores cujas contas estão configuradas com menos direitos de utilização no sistema podem correr menos riscos do que os utilizadores que trabalham com direitos de utilização de administrador. Esta actualização também inclui um kill bit para software produzido pela BackWeb. |
| **Classificação de Gravidade Máxima** | [Moderada](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Impacto da Vulnerabilidade**        | Execução Remota de Código                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Detecção**                          | O Microsoft Baseline Security Analyzer pode detectar se o seu sistema informático necessita desta actualização. A actualização pode requerer um reinício.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Software Afectado**                 | **Microsoft Windows.** Para obter mais informações consulte a secção Localizações do Software Afectado e das Transferências.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |

Localizações do Software Afectado e das Transferências
------------------------------------------------------

<span></span>
**Como utilizar esta tabela?**

Utilize esta tabela para saber mais sobre as actualizações de segurança que poderá ter de instalar. Deverá rever cada programa ou componente de software listado, para ver se é necessário instalar alguma actualizações de segurança. Se alguma aplicação ou componente de software estiver na lista, é fornecida uma hiperligação para a actualização de software disponível e é também a apresentada a classificação da gravidade da actualização de software.

**Nota** Poderá ter que instalar diversas actualizações de segurança para a mesma vulnerabilidade. Reveja toda a coluna para cada identificador de boletim listado, para verificar quais as actualizações que tem que instalar, com base nos programas ou componentes que tem instalados no seu sistema.

#### Sistema Operativo Windows e Servidores

 
<table style="border:1px solid black;">
<caption>Microsoft Windows 2000</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identificador do Boletim</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Classificação de Gravidade Máxima dos Boletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Moderada</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=88990b23-d37f-4d02-a5a3-2ee389ade53c">Microsoft Internet Explorer 5.01 Service Pack 4</a><br />
(Importante)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c47cf8a-8100-4d43-855a-f225a3492b19">Microsoft Internet Explorer 6 Service Pack 1</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=65640123-a9e4-455c-a51a-9df28bd2d412">DirectX 7.0</a><br />
(Crítica)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c6a28d45-13cf-48c4-8f89-3417d552e90b">DirectX 8.1</a><br />
(Crítica)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4dc47e04-5e95-4636-a814-3f912d961461">DirectX 9.0, DirectX 9.0a, DirectX 9.0b ou DirectX 9.0c</a><br />
(Crítica)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cedfd988-232c-4cba-ac65-beb54b8946e0">Microsoft Windows 2000 Service Pack 4</a><br />
(Moderada)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Windows 2000 Server Service Pack 4</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=aa8aa79f-c2cc-440c-9e5c-089143e6f814">Microsoft Windows 2000 Server Service Pack 4</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=53438880-9ea9-4975-9b85-2a1d3d232793">Active Directory</a><br />
(KB949014)<br />
(Importante)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
</tr>
</tbody>
</table>

 
<table style="border:1px solid black;">
<caption>Windows XP</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identificador do Boletim</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Classificação de Gravidade Máxima dos Boletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Moderada</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Service Pack 2 e Windows XP Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=980bb421-950f-4825-8039-44cc961a47b8">Windows XP Service Pack 2 e Windows XP Service Pack 3</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cc325017-3a48-4475-90e4-0c79a002fce3">Microsoft Internet Explorer 6</a><br />
(Crítica)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=fbc31bde-0bf5-490c-96a8-071310d9464a">Windows Internet Explorer 7</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7aaa6427-1e22-4566-960c-836a3b9e5f36">DirectX 9.0, DirectX 9.0a, DirectX 9.0b ou DirectX 9.0c</a><br />
(Crítica)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=36b14a81-5979-4e38-9ba3-ed83dfc17adf">Windows XP Service Pack 2 e Windows XP Service Pack 3</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2d8957c2-e473-4dca-8d68-19fdaea36e26">Windows XP Service Pack 2 e Windows XP Service Pack 3</a><br />
(Moderada)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Professional Service Pack 2 e Windows XP Professional Service Pack 3</td>
<td style="border:1px solid black;">(Consulte a linha Windows XP Service Pack 2 e Windows XP Service Pack 3)</td>
<td style="border:1px solid black;">(Consulte a linha Windows XP Service Pack 2 e Windows XP Service Pack 3)</td>
<td style="border:1px solid black;">(Consulte a linha Windows XP Service Pack 2 e Windows XP Service Pack 3)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7d6aec31-cfb4-470c-983e-78c6a3ebabfe">ADAM</a><br />
(KB949269)<br />
(Moderada)</td>
<td style="border:1px solid black;">(Consulte a linha Windows XP Service Pack 2 e Windows XP Service Pack 3)</td>
<td style="border:1px solid black;">(Consulte a linha Windows XP Service Pack 2 e Windows XP Service Pack 3)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Professional x64 Edition e Windows XP Professional x64 Edition Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=81ab56ca-933f-4974-a393-290a54c30a78">Windows XP Professional x64 Edition e Windows XP Professional x64 Edition Service Pack 2</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c8783cfe-9da5-4842-ab3a-1e2be4fafc47">Microsoft Internet Explorer 6</a><br />
(Crítica)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=19c0ccdc-95c9-4151-96b6-4f49b594ebe0">Windows Internet Explorer 7</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5e8e7e9d-828d-442c-acac-8d91e80dfb36">DirectX 9.0, DirectX 9.0a, DirectX 9.0b ou DirectX 9.0c</a><br />
(Crítica)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ef2e0b48-1bde-4ccc-8f40-2918c2568b2b">ADAM</a><br />
(KB949269)<br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9e9d24ee-8183-428c-8067-168a8d85eaa1">Windows XP Professional x64 Edition e Windows XP Professional x64 Edition Service Pack 2</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=62874096-7d17-4116-9795-4756e2fb6dae">Windows XP Professional x64 Edition e Windows XP Professional x64 Edition Service Pack 2</a><br />
(Moderada)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2003</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identificador do Boletim</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Classificação de Gravidade Máxima dos Boletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Moderada</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Service Pack 1 e Windows Server 2003 Service Pack 2</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=286aada6-a358-41f1-b81a-8de39b9f908a">Microsoft Internet Explorer 6</a><br />
(Moderada)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a1ae9ad2-8329-4c96-b950-7534b3287eaa">Windows Internet Explorer 7</a><br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2274ecb2-2802-47e2-84fd-6621fcb17758">DirectX 9.0, DirectX 9.0a, DirectX 9.0b ou DirectX 9.0c</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=08fc90d5-23aa-4327-8aef-16bc5170769d">Windows Server 2003 Service Pack 1 e Windows Server 2003 Service Pack 2</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a4aed117-3c76-4d80-b50e-8e07e2ef2f7d">Active Directory</a><br />
(KB949014)<br />
(Moderada)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=0a983ffb-4f5a-4b78-9bf5-813dcc5df8d3">ADAM</a><br />
(KB949269)<br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1e8e2faf-009f-403b-a5fe-a47cf014db3a">Windows Server 2003 Service Pack 1 e Windows Server 2003 Service Pack 2</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=dadead99-09cb-4f2b-850d-e98a627cb9f8">Windows Server 2003 Service Pack 1 e Windows Server 2003 Service Pack 2</a><br />
(Baixo)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition e Windows Server 2003 x64 Edition Service Pack 2</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6604569a-3db0-47e7-bd30-7dfba8145386">Microsoft Internet Explorer 6</a><br />
(Moderada)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=fb0c70b4-ce9f-43d6-875a-3cfd0d3a2681">Windows Internet Explorer 7</a><br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5ba63bb7-ed6d-4c59-88b3-456eda07e190">DirectX 9.0, DirectX 9.0a, DirectX 9.0b ou DirectX 9.0c</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=71675ae8-d60a-4834-b358-2d8e761e62fc">Windows Server 2003 x64 Edition e Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8298a6e4-d3e2-48ea-ac29-aa4dc5a8ec77">Active Directory</a><br />
(KB949014)<br />
(Moderada)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=334252db-4a7a-4161-bb71-2a20c0b5bd93">ADAM</a><br />
(KB949269)<br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=78bf92d8-63c4-4596-8425-8fcfea7f5582">Windows Server 2003 x64 Edition e Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=84f9b533-b0cb-46d1-b4a8-5c9469abbd22">Windows Server 2003 x64 Edition e Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Baixo)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 com SP1 para sistemas baseados em Itanium e Windows Server 2003 com SP2 para sistemas baseados em Itanium</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0262beb8-1eb5-4c2d-a50a-0c6c6e0c1f61">Microsoft Internet Explorer 6</a><br />
(Moderada)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=28d2913c-1c6b-4671-9892-de08698cd5a6">Windows Internet Explorer 7</a><br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=be71c002-2f64-49e9-9f4b-ba99c4f3caf6">DirectX 9.0, DirectX 9.0a, DirectX 9.0b ou DirectX 9.0c</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=87affdc9-d9fe-413c-af30-f3d3b671ec72">Windows Server 2003 com SP1 para sistemas baseados em Itanium e Windows Server 2003 com SP2 para sistemas baseados em Itanium</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=f6bf4b85-b91d-4378-a356-cd11f12cbbfd">Active Directory</a><br />
(KB949014)<br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5b7e94fa-22ed-4f7c-b452-647b2e620113">Windows Server 2003 com SP1 para sistemas baseados em Itanium e Windows Server 2003 com SP2 para sistemas baseados em Itanium</a><br />
(Importante)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ac35ce19-d761-4529-9f55-1e1b5b2447ad">Windows Server 2003 com SP1 para sistemas baseados em Itanium e Windows Server 2003 com SP2 para sistemas baseados em Itanium</a><br />
(Baixo)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Vista</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identificador do Boletim</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Classificação de Gravidade Máxima dos Boletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Moderada</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Vista e Windows Vista Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6524debe-be50-44d1-8543-af0bfaf086ad">Windows Vista e Windows Vista Service Pack 1</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6d68b39d-157f-4c3d-ac76-bc5a9386db59">Windows Internet Explorer 7</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4d4b305b-57f8-448d-92fa-3dcdd1f42ed7">DirectX 10.0</a><br />
(Crítica)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ef2d2a4b-4831-41be-b5d0-8df5b01fd205">Windows Vista e Windows Vista Service Pack 1</a><br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4af6575e-b061-45a6-b3d8-ecb32d76b2d3">Windows Vista e Windows Vista Service Pack 1</a><br />
(Moderada)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Vista x64 Edition e Windows Vista x64 Edition Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6adee8b9-3455-4f3b-8bdd-2585c8ff83b8">Windows Vista x64 Edition e Windows Vista x64 Edition Service Pack 1</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4cf92235-861e-4b74-bee3-8e977c8688d9">Windows Internet Explorer 7</a><br />
(Crítica)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b040cfad-2290-44f4-8f5a-5d1ed98a7265">DirectX 10.0</a><br />
(Crítica)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0839fcf4-85ca-445e-896b-f634b10b6700">Windows Vista x64 Edition e Windows Vista x64 Edition Service Pack 1</a><br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=67576acb-9cb6-4c76-9a72-dc5e5556b658">Windows Vista x64 Edition e Windows Vista x64 Edition Service Pack 1</a><br />
(Moderada)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2008</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identificador do Boletim</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Classificação de Gravidade Máxima dos Boletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Crítica</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Importante</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Moderada</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 para sistemas de 32 bits</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a8922e7e-9264-4e09-b8ad-c5420fed8690">Windows Internet Explorer 7</a><br />
(Moderada)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c0c495f8-2a35-4638-a635-1e55dd15e062">DirectX 10.0</a><br />
(Crítica)<strong>**</strong></td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2981156e-2e2f-469e-91be-da127d50f3fc">Active Directory</a><br />
(KB949014)<br />
(Moderada)<strong>*</strong><br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=2981156e-2e2f-469e-91be-da127d50f3fc">AD LDS</a><br />
(KB949014)<br />
(Moderada)<strong>*</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0466a6e7-fdca-4647-af62-449e5f20d1e4">Windows Server 2008 para sistemas de 32 bits</a><br />
(Moderada)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8a507fba-8c93-4952-91e4-98e9e7affbd2">Windows Server 2008 para sistemas de 32 bits</a><br />
(Baixa)<strong>***</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2008 para sistemas baseados em x64</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=05b0e838-24d7-4387-b069-2604bbcc43b9">Windows Internet Explorer 7</a><br />
(Moderada)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0b70fc2e-4e80-4ae8-8682-41ea04c24e4e">DirectX 10.0</a><br />
(Crítica)<strong>**</strong></td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b5cfe6f4-c5ba-4be9-a6b8-9381c40c85aa">Active Directory</a><br />
(KB949014)<br />
(Moderada)<strong>*</strong><br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=b5cfe6f4-c5ba-4be9-a6b8-9381c40c85aa">AD LDS</a><br />
(KB949014)<br />
(Moderada)<strong>*</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=304898e6-21a7-476f-b9ed-7ac0d88a91e2">Windows Server 2008 para sistemas baseados em x64</a><br />
(Moderada)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1a11499d-a008-407f-9084-a5189fa27015">Windows Server 2008 para sistemas baseados em x64</a><br />
(Baixa)<strong>***</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 para sistemas baseados em Itanium</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=640e1865-ebcc-4d69-a770-fd360020da1e">Windows Internet Explorer 7</a><br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=80ec83e0-cfb8-4a5e-9254-6679a7225b83">DirectX 10.0</a><br />
(Crítica)</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;">Não aplicável</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8907783b-e3fe-40b2-9fc8-4937e7d58b7e">Windows Server 2008 para sistemas baseados em Itanium</a><br />
(Moderada)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=59b1689c-e723-4d87-973e-4beac107a6f7">Windows Server 2008 para sistemas baseados em Itanium</a><br />
(Baixo)</td>
</tr>
</tbody>
</table>
 

**\*Instalação Server Core do Windows Server 2008 afectada.** Para edições suportadas do Windows Server 2008, esta actualização aplica-se com a mesma classificação de gravidade, quer o Windows Server 2008 tenha ou não sido instalado utilizando a opção de instalação Server Core. Para mais informações sobre esta opção de instalação, consulte a informação sobre [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalação Server Core do Windows Server 2008 não afectada.** As vulnerabilidades corrigidas por esta actualização não afectam edições suportadas do Windows Server 2008 se este tiver sido instalado usando a opção de instalação Server Core. Para mais informações sobre esta opção de instalação, consulte a informação sobre [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*A instalação Server Core do Windows Server 2008 não é afectada, mas receberá esta actualização.** As vulnerabilidades corrigidas por esta actualização não afectam as edições suportadas do Windows Server 2008 se este tiver sido instalado usando a opção de instalação Server Core, apesar de os ficheiros afectados pelas vulnerabilidades poderem estar presentes no sistema. Contudo, os utilizadores com ficheiros afectados continuarão a receber esta actualização porque os ficheiros actualizados são mais recentes (com números de versão superiores) do que os ficheiros actualmente no seu sistema. Para mais informações sobre esta opção de instalação, consulte a informação sobre [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Tenha em atenção que a opção de instalação Server Core não se aplica a determinadas edições do Windows Server 2008; consulte [Comparar as Opções de Instalação Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Orientações e ferramentas de detecção e implementação
-----------------------------------------------------

<span></span>
**Centro de segurança**

Faça a gestão do software e actualizações de segurança de que necessita para implementação em servidores, ambientes de trabalho e computadores portáteis na sua organização. Para mais informações, visite o [Centro de Gestão de Actualizações TechNet](http://go.microsoft.com/fwlink/?linkid=69903). O [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) fornece informações adicionais sobre segurança em produtos Microsoft. Os clientes podem visitar o site de [Segurança em casa](http://go.microsoft.com/fwlink/?linkid=85102), no qual podem consultar esta informação ao clicarem em “Actualizações de segurança recentes”.

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

### Outras informações

#### Ferramenta de Remoção de Software Malicioso Windows

A Microsoft publicou uma versão actualizada da Ferramenta de Remoção de Software Malicioso para o Microsoft Windows no Windows Update, no Microsoft Update, no Windows Server Update Services e no Centro de Transferências.

#### Actualizações não relacionadas com segurança, de elevada prioridade, no MU, WU e WSUS

Para obter informações não relacionadas com segurança de publicações sobre o Windows Update e Microsoft update, consulte:

-   [Artigo 894199 da Base de Dados de Conhecimento da Microsoft](http://support.microsoft.com/kb/894199): Descrição das alterações de conteúdo do Software Update Services e Windows Server Update Services para 2008. Inclui todos os conteúdos do Windows.
-   [Actualizações Novas, Revistas e Publicadas para Produtos Microsoft que não Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

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

-   Sebastian Apelt, Peter Vreugdenhil e um investigador anónimo, a trabalhar com a [Tipping Point](http://www.tippingpoint.com/) e a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecerem informações sobre uma questão descrita no boletim MS08-031.
-   Mark Dowd, investigador da [IBM Internet Security Systems X-Force](http://xforce.iss.net/), por fornecer informações sobre uma questão descrita no boletim MS08-033.
-   Investigador anónimo, a trabalhar com a [Tipping Point](http://www.tippingpoint.com/) e a [Zero Day Initiative](http://www.zerodayinitiative.com/), por fornecer informações sobre uma questão descrita no boletim MS08-033.
-   Alex Matthews e John Guzik, da [Securify](http://www.securify.com/), por fornecerem informações sobre uma questão descrita no boletim MS08-035.

#### Assistência

-   O software afectado incluído neste boletim foi testado para determinar quais as versões afectadas. As outras versões ultrapassaram o respectivo ciclo de vida de suporte. Para determinar o ciclo de vida de suporte da versão do seu software, visite o [Web site do Ciclo de Vida de Suporte Microsoft](http://support.microsoft.com/lifecycle/).
-   Os clientes nos E.U.A. e no Canadá podem receber suporte técnico a partir do Web site de [Suporte Técnico da Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) em 1-866-PCSAFETY. As chamadas de suporte técnico associadas a actualizações de segurança são gratuitas.
-   Os clientes internacionais podem receber suporte das subsidiárias locais da Microsoft. O suporte técnico associado às actualizações de segurança é gratuito. Para mais informações sobre como contactar a Microsoft relativamente a questões de suporte, visite o [Web site de Suporte Internacional](http://go.microsoft.com/fwlink/?linkid=21155).

#### Exclusão de garantia

As informações fornecidas na Base de Dados de Conhecimento da Microsoft são fornecidas "tal como estão", sem garantias de qualquer tipo. A Microsoft exclui todas as garantias, sejam expressas ou implícitas, incluindo as garantias de comercialização e adequação a um fim específico. Em caso algum serão a Microsoft Corporation ou os seus fornecedores responsáveis por quaisquer prejuízos, incluindo prejuízos directos, indirectos, incidentais ou consequentes, extraordinários ou por perda de lucros negociais, ainda que a Microsoft Corporation, ou os seus fornecedores tenham sido notificados da possibilidade de ocorrência de tais prejuízos. A exclusão ou limitação de responsabilidade por prejuízos consequentes ou incidentais não é permitida em alguns estados ou jurisdições, pelo que a limitação supra poderá não ser aplicável.

#### Revisões

-   V1.0 (10 de Junho de 2008): Publicação do Resumo dos Boletins.
-   V1.1 (11 de Junho de 2008): Correcção da tabela de Software Afectado para o Windows XP, com o objectivo de clarificar as entradas para o Windows XP Service Pack 2 e Windows XP Service Pack 3 nos boletins MS08-030, MS08-031, MS08-032, MS08-033 e MS08-036.
-   V2.0 (16 de Julho de 2008): DirectX 9.0a adicionado como software afectado para o boletim MS08-033.
-   V2.1 (1 de Abril de 2009): Para o boletim MS08-032, esclarecido que as instalações Server Core do Windows Server 2008 não são afectadas pela vulnerabilidade discutida neste boletim, mas receberão esta actualização. Trata-se de uma alteração informativa apenas. Os utilizadores destas instalações não necessitam de instalar esta actualização.

*Built at 2014-04-18T01:50:00Z-07:00*
