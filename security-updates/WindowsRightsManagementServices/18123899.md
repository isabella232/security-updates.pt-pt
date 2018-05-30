---
TOCTitle: Contas e Permissões Necessárias para o RMS
Title: Contas e Permissões Necessárias para o RMS
ms:assetid: '07a51daa-6823-41e6-b453-92f1a0592361'
ms:contentKeyID: 18123899
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720178(v=WS.10)'
---

Contas e Permissões Necessárias para o RMS
==========================================

A tabela seguinte especifica os direitos e permissões do utilizador necessários para implementar e administrar o RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Actividade</th>
<th>Contas e Permissões de Utilizador</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Instalar o RMS</td>
<td style="border:1px solid black;">Inicie a sessão utilizando uma conta de domínio que seja membro do grupo de Administradores local.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aprovisionar o RMS</td>
<td style="border:1px solid black;">Inicie a sessão utilizando uma conta de domínio que seja membro do grupo de Administradores local. Além disso, a conta que está a ser visualizada tem de ter um início de sessão SQL com o papel de Administrador do Sistema concedido na base de dados do Servidor SQL para que o RMS possa definir as bases de dados.
Durante o aprovisionamento, é necessário especificar a conta de serviço do RMS, que já deve ter sido criada. A conta deverá ser uma conta de utilizador de domínio padrão, sem permissões adicionais. Esta conta passa a ser membro do Grupo de Serviços do RMS e é a conta que vai ser executada pelo RMS em condições normais de funcionamento.
Em implementações com um só servidor nas quais a base de dados se encontra no mesmo computador que o servidor de certificações de raiz, pode especificar a conta de Sistema Local. No entanto, por questões de segurança, recomenda-se que seja sempre especificada a conta de serviço do RMS em vez da conta de Sistema Local. Quando a base de dados se encontra num servidor à parte, é necessário especificar a conta de serviço do RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Administrar o RMS</td>
<td style="border:1px solid black;">Inicie a sessão utilizando uma conta de domínio que seja membro do grupo de Administradores local. Pode personalizar as definições de segurança para gerir o acesso às páginas Web de administração.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720178.note(WS.10).gif)Nota                                                                                                                                                                                                                                                                       |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A conta utilizada para iniciar sessão no servidor do RMS não requer membros adicionais de grupo de domínio, como o grupo Admins do domínio. No entanto, algumas tarefas administrativas específicas, como o registo do ponto de ligação do serviço e a modificação das políticas de segurança, exigem uma conta com privilégios adicionais. |
