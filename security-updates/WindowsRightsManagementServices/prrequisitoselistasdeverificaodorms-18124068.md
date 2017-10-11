---
TOCTitle: 'Pré-requisitos e Listas de Verificação do RMS'
Title: 'Pré-requisitos e Listas de Verificação do RMS'
ms:assetid: '836d96ef-d0fd-4935-b595-e8dec19cbb2b'
ms:contentKeyID: 18124068
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747582(v=WS.10)'
---

Pré-requisitos e Listas de Verificação do RMS
=============================================

Antes de iniciar a instalação do RMS, reveja os pré-requisitos de tecnologia para a utilização do RMS. Cada uma das tecnologias listadas está integrada no RMS pelo que necessita de obter um conhecimento básico sobre o seu funcionamento para implementar o RMS com êxito. A utilização das listas de verificação seguintes ajudam-no a criar listas de tarefas e planos de implementação e administração do RMS:

-   [Pré-requisitos da Tecnologia](#bkmk_9)
-   [Lista de Verificação da Implementação do RMS](#bkmk_10)
-   [Listas de Verificação da Administração do RMS](#bkmk_14)

<span id="BKMK_9"></span>
Pré-requisitos da Tecnologia
----------------------------

Esta colecção de documentação fornece informações que o ajudam a compreender o funcionamento do Windows RMS, como planear e executar uma implementação na organização e como administrar o sistema diariamente. Parte do princípio de que já está familiarizado com as seguintes áreas:

-   Implementação e administração do Windows Server 2003
-   Implementação e administração do Active Directory
-   Implementação e administração dos Serviços de Informação Internet 6.0 (IIS) da Microsoft®
-   Administração do Microsoft® SQL Server™ 2000
-   Conceitos básicos sobre a infra-estrutura de chaves públicas (PKI)
-   Redes e segurança de servidores

Para mais informações sobre estes tópicos, consulte "Recursos Adicionais" em [Utilizar um Servidor do RMS](http://go.microsoft.com/fwlink/?linkid=42495) nesta colecção de documentação.

<span id="BKMK_10"></span>
Lista de Verificação da Implementação do RMS
--------------------------------------------

Esta secção fornece listas de verificação para as seguintes tarefas de implementação:

-   [Implementar uma Instalação de Servidor Único](#bkmk_11)
-   [Implementar Clusters de Certificações de Raiz e de Licenciamento](#bkmk_12)
-   [Implementar o RMS nas Florestas](#bkmk_13)

Para mais informações sobre a implementação do RMS, consulte [Implementar um Sistema do RMS](http://go.microsoft.com/fwlink/?linkid=42494) nesta colecção de documentação.

<span id="BKMK_11"></span>
Implementar uma Instalação de Servidor Único
--------------------------------------------

Utilize a lista de verificação seguinte para implementar um servidor único do RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Passo</th>
<th>Referência</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Reveja os conceitos e as informações de planeamento.</td>
<td style="border:1px solid black;">&quot;Preparar uma Implementação do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Reveja os requisitos de sistema e verifique se o hardware e o software necessários estão disponíveis.</td>
<td style="border:1px solid black;">&quot;Pré-requisitos de Infra-estrutura para o RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planear uma Implementação do RMS</a>.
&quot;Planear a Infra-estrutura de Servidores de Bases de Dados&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planear uma Implementação do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Configure a infra-estrutura, incluindo os pré-requisitos de hardware e software, as contas administrativas e o suporte de SMS ou de Política de Grupo, conforme apropriado.</td>
<td style="border:1px solid black;">&quot;Preparar uma Implementação do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Instale e configure o RMS no servidor.</td>
<td style="border:1px solid black;">&quot;Configurar Serviços de Certificação e Licenciamento no Primeiro Servidor&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Teste a implementação.</td>
<td style="border:1px solid black;">&quot;Configurar um Ambiente de Teste&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Implemente o RMS no ambiente de produção.</td>
<td style="border:1px solid black;">&quot;Definir o âmbito da Implementação do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_12"></span>
Implementar Clusters de Certificações de Raiz e de Licenciamento  
----------------------------------------------------------------
  
Utilize a lista de verificação seguinte para implementar clusters de certificações de raiz e de licenciamento.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Passo</th>
<th>Referência</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Reveja os conceitos e as informações de planeamento.</td>
<td style="border:1px solid black;">&quot;Preparar uma Implementação do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Reveja os requisitos de sistema e verifique se o hardware e o software necessários estão disponíveis.</td>
<td style="border:1px solid black;">&quot;Pré-requisitos de Infra-estrutura para o RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planear uma Implementação do RMS</a>.
&quot;Planear a Infra-estrutura de Servidores de Bases de Dados&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planear uma Implementação do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Reveja o plano de implementação para compreender a topologia e os componentes que vão ser instalados.</td>
<td style="border:1px solid black;">&quot;Determinar a Topologia do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planear uma Implementação do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Configure a infra-estrutura, incluindo os pré-requisitos de hardware e software, contas administrativas e suporte de SMS ou de Política de Grupo, conforme apropriado.</td>
<td style="border:1px solid black;">&quot;Preparar uma Implementação do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Instale e configure o RMS nos servidores do cluster de certificações de raiz.</td>
<td style="border:1px solid black;">&quot;Configurar Serviços de Certificação e Licenciamento no Primeiro Servidor&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.
&quot;Adicionar Servidores para Suportar a Certificação e o Licenciamento&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Instale e configure o RMS nos servidores do cluster de licenciamento.</td>
<td style="border:1px solid black;">&quot;Configurar Serviços de Certificação e Licenciamento no Primeiro Servidor&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.
&quot;Adicionar Servidores para Suportar a Certificação e o Licenciamento&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Configure o balanceamento de carga.</td>
<td style="border:1px solid black;">&quot;Expandir a infra-estrutura Básica para Suportar Clusters&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Teste a implementação.</td>
<td style="border:1px solid black;">&quot;Configurar um Ambiente de Teste&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Implemente o RMS no ambiente de produção.</td>
<td style="border:1px solid black;">&quot;Definir o âmbito da Implementação do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_13"></span>
Implementar o RMS nas Florestas  
-------------------------------
  
Utilize a lista de verificação seguinte para implementar o RMS raiz nas florestas.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Passo</th>
<th>Referência</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Reveja os conceitos e as informações de planeamento.</td>
<td style="border:1px solid black;">&quot;Preparar uma Implementação do RMS&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Configure as permissões necessárias com base no modelo de fidedignidade.</td>
<td style="border:1px solid black;">&quot;Implementar o RMS nas Florestas&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Defina os atributos adequados do Active Directory para as florestas.</td>
<td style="border:1px solid black;">&quot;Implementar o RMS nas Florestas&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_14"></span>
Listas de Verificação da Administração do RMS  
---------------------------------------------
  
Esta secção fornece listas de verificação para as seguintes tarefas de administração:
  
-   [Implementar um Modelo de Política de Direitos](#bkmk_15)  
-   [Implementar um Cliente Novo do RMS](#bkmk_16)  
-   [Adicionar um Domínio de Utilizador Fidedigno](#bkmk_17)  
-   [Adicionar um Domínio de Publicação Fidedigno](#bkmk_18)
  
Para mais informações sobre a gestão do RMS, consulte [Utilizar um Servidor do RMS](http://go.microsoft.com/fwlink/?linkid=42495) nesta colecção de documentação.
  
<span id="BKMK_15"></span>
Implementar um Modelo de Política de Direitos  
---------------------------------------------
  
Utilize a lista de verificação seguinte para implementar um modelo de política de direitos.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Passo</th>
<th>Referência</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Reveja os conceitos relevantes.</td>
<td style="border:1px solid black;">&quot;Modelos de Políticas de Direitos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42496">Referência Técnica do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Especifique a localização do modelo de política de direitos.</td>
<td style="border:1px solid black;">&quot;Para Especificar a Localização dos Modelos de Políticas de Direitos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Crie o modelo de política de direitos.</td>
<td style="border:1px solid black;">&quot;Criar e Modificar Modelos de Políticas de Direitos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.
&quot;Para Adicionar um Modelo de Política de Direitos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Distribua o modelo de política de direitos.</td>
<td style="border:1px solid black;">&quot;Distribuir Modelos de Políticas de Direitos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_16"></span>
Implementar um Cliente Novo do RMS  
----------------------------------
  
Utilize a lista de verificação seguinte para implementar uma versão nova do cliente do RMS.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Passo</th>
<th>Referência</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Reveja os conceitos relevantes.</td>
<td style="border:1px solid black;">&quot;Planeamento da Distribuição do Cliente&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42494">Implementar um Sistema do RMS</a>
&quot;Excluir Versões do Cofre&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Para forçar a actualização de todos os clientes para a versão mais recente do cliente, exclua a versão desactualizada do cofre.</td>
<td style="border:1px solid black;">&quot;Para Excluir Versões do Cofre&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_17"></span>
Adicionar um Domínio de Utilizador Fidedigno  
--------------------------------------------
  
Utilize a lista de verificação seguinte para adicionar um domínio de utilizador fidedigno.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Passo</th>
<th>Referência</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Reveja os conceitos relevantes.</td>
<td style="border:1px solid black;">&quot;Domínios de Utilizadores Fidedignos&quot; na <a href="http://go.microsoft.com/fwlink/?linkid=42496">Referência Técnica do RMS</a>.
&quot;Adicionar e Remover Domínios de Utilizadores Fidedignos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Obtenha o certificado de licenciador de servidores do domínio de utilizador que pretende adicionar. (O administrador da instalação fidedigna deverá facultar o certificado.) Em seguida, adicione o domínio de utilizador à instalação.</td>
<td style="border:1px solid black;">&quot;Para Adicionar um Domínio de Utilizadores Fidedignos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_18"></span>
Adicionar um Domínio de Publicação Fidedigno  
--------------------------------------------
  
Utilize a lista de verificação seguinte para adicionar um domínio de publicação fidedigno.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Passo</th>
<th>Referência</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Reveja os conceitos relevantes.</td>
<td style="border:1px solid black;">&quot;Domínios de Publicação Fidedignos&quot; na <a href="http://go.microsoft.com/fwlink/?linkid=42496">Referência Técnica do RMS</a>.
&quot;Adicionar e Remover Domínios de Publicação Fidedignos&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Obtenha o certificado de licenciador de servidores encriptado e a chave privada do domínio de publicação que pretende adicionar e, em seguida, adicione o domínio de publicação à instalação.</td>
<td style="border:1px solid black;">&quot;Para Adicionar um Domínio de Publicação Fidedigno&quot; em <a href="http://go.microsoft.com/fwlink/?linkid=42495">Utilizar um Servidor do RMS</a>.</td>
</tr>
</tbody>
</table>
