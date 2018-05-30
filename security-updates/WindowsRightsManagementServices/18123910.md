---
TOCTitle: Criar Listas de Revogações
Title: Criar Listas de Revogações
ms:assetid: '1ef75199-3344-4225-84de-a863a777696a'
ms:contentKeyID: 18123910
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720208(v=WS.10)'
---

Criar Listas de Revogações
==========================

A implementação de revogações requer a distribuição de uma lista de revogações, que é um documento XML que utiliza a linguagem XrML (eXtensible Rights Markup Language) e lista os principais que já não devem ter acesso ao conteúdo protegido. Têm de ser criadas listas de revogações que estejam marcadas com a hora e devidamente assinadas, utilizando a ferramenta de Assinatura da Lista de Revogações (RLsigner.exe) fornecida com o RMS.

| ![](/security-updates/images/Cc720208.Important(WS.10).gif)Importante                                                               |
|------------------------------------------------------------------------------------------------------------------------------------------------|
| Para assinar a lista de revogações utilizando o RLsigner.exe, é necessário guardar o ficheiro da lista de revogações como um ficheiro unicode. |

Exemplo de Lista de Revogações
------------------------------

Este tópico apresenta um exemplo de uma lista de revogações completa, explicando cada um dos possíveis mecanismos de revogação. Este exemplo pode ser utilizado como modelo para criar outras listas de revogações.

Uma lista de revogações é um ficheiro XML que utiliza a linguagem XrML.

O elemento BODY contém quatro elementos subordinados:

-   **ISSUEDTIME**. Contém a data e hora de emissão da lista de revogações. O RLsigner.exe insere este elemento no ficheiro; o elemento é fornecido no exemplo apenas para demonstrar a estrutura global do ficheiro da lista de revogações.
-   **DESCRIPTOR**. Contém dados que identificam o ficheiro como sendo uma lista de revogações.
-   **ISSUER**. Contém dados que identificam a entidade que emite a lista de revogações.
-   **REVOCATIONLIST**. Contém elementos subordinados REVOKE que especificam entidades que são revogadas por esta lista.

Abaixo é apresentada uma amostra de um ficheiro de lista de revogações.

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Nota                                                          |
|--------------------------------------------------------------------------------------------------------------------------------|
        ```
| ![](/security-updates/images/Cc720208.Caution(WS.10).gif)Atenção                                                                        |
|----------------------------------------------------------------------------------------------------------------------------------------------------|
| Ao especificar o URL na lista de revogações, deixa de ser suportado um caminho UNS no RMS com SP1 ou RMS com SP2. Será necessário utilizar um URL. |

Depois de ter definido os elementos REVOKE, a lista de revogações fica pronta para ser assinada.

Utilizar o Elemento REVOKE
--------------------------

Na lista de revogações exemplificativa, na secção Exemplo de Lista de Revogações, cada elemento REVOKE especifica um principal que será revogado. A etiqueta de abertura tem atributos de categoria e de tipo que definem aquilo que está a ser revogado e qual o critério de identificação. Diferentes elementos REVOKE têm diferentes elementos subordinados, dependendo da acção que é especificada pelos atributos de categoria e de tipo.

Para mais informações acerca da especificação dos elementos REVOKE, consulte os seguintes exemplos:

-   [Revogar Principais com Base numa Chave Pública](#bkmk_1)
-   [Revogar Certificados e Licenças com Base no GUID](#bkmk_2)
-   [Revogar Certificados e Licenças com Base no Valor Hash](#bkmk_3)
-   [Revogar Certificados e Licenças com Base na Chave Pública do Emissor](#bkmk_4)
-   [Revogar Certificados e Licenças com Base na ID do Emissor](#bkmk_5)
-   [Revogar Conteúdo com Base na ID do Conteúdo](#bkmk_6)
-   [Revogar Certificados com Base na ID do Principal](#bkmk_10)
-   [Revogar Principais com Base no Windows Live ID](#bkmk_7)

<span id="BKMK_1"></span>
#### Revogar Principais com Base numa Chave Pública

        ```

<span id="BKMK_2"></span>
#### Revogar Certificados e Licenças com Base no GUID

        ```
#### Revogar por manifesto de aplicação

Para revogar por manifesto de aplicação, deve extrair a ID do emissor, a chave pública do emissor, a ID de licença ou hash de licença do manifesto de aplicação. No entanto, os manifestos de aplicações estão codificados numa base 64 para que as informações não estejam disponíveis em texto simples. O RMS Software Development Kit (SDK) permite desenvolver um programa através dos métodos DRMConstructCertificateChain, DRMDeconstructCertificateChain e DRMDecode para descodificar o manifesto de aplicação e obter as informações necessárias.

Se pretende impedir a capacidade de uma determinada aplicação consumir o conteúdo protegido, pondere utilizar a exclusão de aplicações para proibir o cluster do RMS de atribuir licenças de utilização a essas aplicações. A limitação da exclusão consiste no facto de não conseguir evitar que alguém com uma licença de utilização válida desencripte o conteúdo protegido. Para mais informações sobre a exclusão de aplicações, consulte a secção sobre [Excluir Aplicações](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) anteriormente nesta secção.

<span id="BKMK_3"></span>
#### Revogar Certificados e Licenças com Base no Valor Hash

        ```
#### Revogar por manifesto de aplicação

Para revogar por manifesto de aplicação, deve extrair a ID do emissor, a chave pública do emissor, a ID de licença ou hash de licença do manifesto de aplicação. No entanto, os manifestos de aplicações estão codificados numa base 64 para que as informações não estejam disponíveis em texto simples. O RMS SDK permite desenvolver um programa através dos métodos DRMConstructCertificateChain, DRMDeconstructCertificateChain e DRMDecode para descodificar o manifesto de aplicação e obter as informações necessárias.

Se pretende impedir a capacidade de uma determinada aplicação consumir o conteúdo protegido, pondere utilizar a exclusão de aplicações para proibir o cluster do RMS de atribuir licenças de utilização a essas aplicações. A limitação da exclusão consiste no facto de não conseguir evitar que alguém com uma licença de utilização válida desencripte o conteúdo do RMS protegido. Para mais informações sobre a exclusão de aplicações, consulte a secção sobre [Excluir Aplicações](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) anteriormente nesta secção.

<span id="BKMK_4"></span>
#### Revogar Certificados e Licenças com Base na Chave Pública do Emissor

        ```

<span id="BKMK_5"></span>
#### Revogar Certificados e Licenças com Base na ID do Emissor

        ```
| ![](/security-updates/images/Cc720208.note(WS.10).gif)Nota                                                                                                                                                                                                           |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Quando especificar o tipo de ID, certifique-se de que não existe qualquer símbolo de retorno entre o identificador exclusivo global (GUID) e a etiqueta de fecho. Se adicionar um símbolo de retorno inadvertidamente, o cliente do RMS não pode analisar a lista de revogação. |

<span id="BKMK_6"></span>
#### Revogar Conteúdo com Base na ID do Conteúdo

        ```
| ![](/security-updates/images/Cc720208.note(WS.10).gif)Nota                                                                                                                                                                                                           |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Quando especificar o tipo de ID, certifique-se de que não existe qualquer símbolo de retorno entre o identificador exclusivo global (GUID) e a etiqueta de fecho. Se adicionar um símbolo de retorno inadvertidamente, o cliente do RMS não pode analisar a lista de revogação. |

<span id="BKMK_10"></span>
#### Revogar Principais com Base na Conta do Windows

        ```
| ![](/security-updates/images/Cc720208.note(WS.10).gif)Nota                                                                                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Quando especificar o tipo de ID, certifique-se de que não existe qualquer símbolo de retorno entre o SID da conta do Windows e a etiqueta de fecho. Se adicionar um símbolo de retorno inadvertidamente, o cliente do RMS não pode analisar a lista de revogação. |

<span id="BKMK_7"></span>
#### Revogar Principais com Base no Windows Live ID

        ```
| ![](/security-updates/images/Cc720208.note(WS.10).gif)Nota                                                                                                                                                                                                              |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Quando especificar o tipo de ID, certifique-se de que não existe qualquer símbolo de retorno entre o identificador exclusivo principal (PUID) e a etiqueta de fecho. Se adicionar um símbolo de retorno inadvertidamente, o cliente do RMS não pode analisar a lista de revogação. |

<span id="BKMK_8"></span>
Inserir uma Assinatura numa Lista de Revogações
-----------------------------------------------

Depois de terminada a criação de uma lista de revogações, é necessário introduzir uma assinatura na lista de revogações, conforme se descreve neste tópico. Poderá disponibilizar a lista de revogações aos utilizadores a partir do URL especificado no modelo de política de direitos associado.

O primeiro passo a utilizar para introduzir uma assinatura consiste em gerar um par de chaves e um ficheiro de chave para a lista de revogações, utilizando a ferramenta Strong Name (Sn.exe). A ferramenta Sn.exe está incluída no Microsoft .NET Framework SDK 1.1, que se encontra disponível no Web site da Microsoft [http://go.microsoft.com/fwlink/?LinkId=104796](http://go.microsoft.com/fwlink/?linkid=104796).

Para assinar o ficheiro da lista de revogações utilizando a ferramenta RLsigner.exe, este terá de ter sido guardado como ficheiro unicode.

**Para utilizar o Sn.exe para gerar um novo par de chaves e escrever esse par num ficheiro**
1.  Crie a chave privada. Numa linha de comandos, escreva o seguinte comando e, em seguida, prima ENTER:

    **sn -k** *ficheiro\_chave\_privada***.snk**

    em que *ficheiro\_chave\_privada* é o nome do ficheiro da chave.

2.  Use o Sn.exe para extrair a chave pública do ficheiro de par de chaves criado no Passo 1 e exporte-a para um ficheiro separado. Escreva o comando que se segue e prima ENTER:

    **sn -p** *ficheiro\_chave\_privada ficheiro\_chave\_pública*

    em que *ficheiro\_chave\_privada* é o nome do ficheiro de chave privada criado no Passo 1 e *ficheiro\_chave\_pública* é o nome do ficheiro em que a chave pública exportada será armazenada.

3.  Altere a extensão do ficheiro de chave privada (criado no Passo 1) de .snk para .dat para utilização com a ferramenta RLsigner.exe.

4.  Use a ferramenta RLsigner.exe para introduzir uma assinatura num ficheiro de lista de revogações. Esta ferramenta faz parte do RMS. Por predefinição, está localizada no directório %systemdrive%\\Program Files\\Windows Rights Management Services\\Tools.

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Nota         |
|-------------------------------------------------------------------------------|
| A ferramenta RLsigner.exe não suporta nomes de ficheiros que incluam espaços. |

<span id="BKMK_9"></span>
Utilizar a ferramenta RLsigner.exe
----------------------------------

Quando se executa a ferramenta RLsigner.exe, esta cria em primeiro lugar uma assinatura, utilizando a chave privada que é fornecida no ficheiro de chave. Depois, cria um ficheiro de saída baseado no ficheiro da lista de revogações fornecido.

| ![](/security-updates/images/Cc720208.Important(WS.10).gif)Importante                                            |
|-----------------------------------------------------------------------------------------------------------------------------|
| Para utilizar a ferramenta RLsigner.exe, o ficheiro da lista de revogações terá de ter sido guardado como ficheiro unicode. |

Para utilizar a ferramenta RLsigner.exe para assinar a lista de revogações, escreva o seguinte comando na linha de comandos:

**rlsigner.exe** *ficheiro\_entrada* **{-f** *ficheiro\_chave* **| -h** *nome\_contentor* **CSP}** *ficheiro\_saída*

Utilize as informações que se seguem para preencher os parâmetros de entrada do comando:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parâmetro</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><em>ficheiro_entrada</em></td>
<td style="border:1px solid black;">Nome do ficheiro da lista de revogações compatível com XrML que foi preparado</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>ficheiro_chave</em></td>
<td style="border:1px solid black;">Nome do ficheiro que contém as chaves pública e privada que foram geradas</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>nome_contentor</em></td>
<td style="border:1px solid black;">Nome do contentor da chave</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>ficheiro_saída</em></td>
<td style="border:1px solid black;">Nome do ficheiro da lista de revogações assinado que vai ser criado pela ferramenta</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720208.note(WS.10).gif)Nota         |  
|-------------------------------------------------------------------------------|  
| A ferramenta RLsigner.exe não suporta nomes de ficheiros que incluam espaços. |
  
Os exemplos que se seguem descrevem a forma como pode ser utilizada a ferramenta RLsigner.exe numa linha de comandos com diferentes fornecedores de serviços criptográficos:
  
-   Exemplo de sintaxe de uma linha de comandos na qual é utilizado um ficheiro de chave:  
    **rlsigner.exe rl.xml -f chave.dat saída.xml**  
-   Exemplo de sintaxe de uma linha de comandos na qual é utilizado um módulo de segurança por hardware:  
    **rlsigner.exe rl.xml -h Contentor CSP saída.xml**
  
A ferramenta RLsigner.exe fornece informações acerca de erros básicos e operações efectuadas com êxito no respectivo código de retorno. A tabela que se segue apresenta uma descrição dos códigos de retorno possíveis.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Código de Retorno</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">0</td>
<td style="border:1px solid black;">Êxito</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-1</td>
<td style="border:1px solid black;">Impossível ler o ficheiro de origem</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-2</td>
<td style="border:1px solid black;">Impossível ler o ficheiro de chave</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-3</td>
<td style="border:1px solid black;">Ficheiro de chave inválido</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-4</td>
<td style="border:1px solid black;">Ficheiro de origem inválido</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-5</td>
<td style="border:1px solid black;">Impossível escrever no ficheiro de saída</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-6</td>
<td style="border:1px solid black;">Erro desconhecido</td>
</tr>
</tbody>
</table>
  
Pode querer programar a assinatura de listas de revogações com base na taxa de actualização especificada para o servidor.
  
É possível automatizar o processo de assinatura da lista de revogações utilizando scripts. O seguinte exemplo de VBScript chama a ferramenta RLSigner.exe e escreve os resultados no registo de eventos do Sistema.
  
<codesnippet asp="http://msdn2.microsoft.com/asp" language displaylanguage="Visual Basic">const EVT\_SUCCESS = 0 const EVT\_ERROR = 1 const EVT\_WARNING = 2 const EVT\_INFORMATION = 4 const EVT\_AUDIT\_SUCCESS = 8 const EVT\_AUDIT\_FAILURE = 16 Dim WshShell, oExec Set WshShell = CreateObject( "WScript.Shell" ) Set oExec = WshShell.Exec("rlsigner.exe input\_file key\_file output\_file") Do While oExec.Status = 0 WScript.Sleep 100 Loop if WshShell.ExitCode &lt;&gt; 0 Then WshShell.LogEvent EVT\_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """" else WshShell.LogEvent EVT\_SUCCESS, "RLsigner completed successfully" end if  
```
