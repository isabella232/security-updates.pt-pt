---
TOCTitle: 'FAQ sobre o RMS: Modelos de Política de Direitos'
Title: 'FAQ sobre o RMS: Modelos de Política de Direitos'
ms:assetid: '01515f08-9844-4c1a-9ab5-a5a60a901b50'
ms:contentKeyID: 18123893
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720175(v=WS.10)'
---

FAQ sobre o RMS: Modelos de Política de Direitos
================================================

Perguntas Mais Frequentes Sobre os Modelos do RMS
-------------------------------------------------

-   [Posso impor um modelo de RMS predefinido para todos os conteúdos criados numa organização para que uma empresa possa garantir um conjunto mínimo de direitos?](#bkmk_57)
-   [Em que local estão os modelos de políticas do RMS?](#bkmk_58)
-   [Quando os modelos são criados, o alias dos utilizadores e as listas de distribuição (DLs) são associados aos modelos. De que forma uma organização com vários departamentos pode fornecer modelos com os mesmos direitos básicos, mas conceder esses direitos a diferentes grupos dependendo do conteúdo?](#bkmk_59)
-   [Os direitos são aplicados a um documento estático? Se um ficheiro for enviado e os direitos necessitarem de ser alterados posteriormente, isto pode ser efectuado com a licença de publicação incorporada no ficheiro e não no servidor de "políticas" do RMS?](#bkmk_60)

<span id="BKMK_57"></span>
#### Posso impor um modelo de RMS predefinido para todos os conteúdos criados numa organização para que uma empresa possa garantir um conjunto mínimo de direitos?

Sim. O RMS SDK permite desenvolver uma aplicação personalizada que pode impor os modelos que forem necessários. No entanto, a implementação da Gestão de Direitos de Informação do Office 2003 e posteriores não suporta a imposição de modelos no conteúdo.

<span id="BKMK_58"></span>
#### Em que local estão os modelos de políticas do RMS?

A localização dos modelos é determinada pela aplicação activada pelo RMS. Para o Office 2003 e posteriores, é guardada como uma definição do utilizador no registo, na seguinte localização:

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\11.0\\Common\\DRM\\AdminTemplatePath**

- ou -

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\12.0\\Common\\DRM\\AdminTemplatePath** para o Microsoft Office 2007.

| ![](images/Cc720175.note(WS.10).gif)Nota                                                                                                                                                                |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se esta entrada apontar para uma pasta local no cliente, os ficheiros dos modelos deverão ser copiados para o cliente. Se esta apontar para uma pasta partilhada na rede, não estará disponível quando o utilizador estiver offline. |

<span id="BKMK_59"></span>
#### Quando os modelos são criados, o alias dos utilizadores e as listas de distribuição (DLs) são associados aos modelos. De que forma uma organização com vários departamentos pode fornecer modelos com os mesmos direitos básicos, mas conceder esses direitos a diferentes grupos dependendo do conteúdo?

Existem duas soluções para este cenário:

-   Crie um modelo individual denominado “Confidencial Empresa”, que é licenciado para todos os funcionários da unidade empresarial e, em seguida, utilize esse modelo no correio electrónico e envie a mensagem de correio electrónico para as pessoas específicas. A vantagem é que é necessário um modelo individual para cada unidade empresarial para o correio electrónico e pode restringir-se aos utilizadores a quem se envia. A desvantagem é que qualquer pessoa exterior ao grupo a quem foi enviado originalmente ainda poderá lê-lo.
-   Em alternativa, crie vários modelos, incluindo um para cada lista de distribuição. Embora forneça um controlo muito mais preciso, significa também que o departamento de TI deverá suportar vários modelos.

<span id="BKMK_60"></span>
#### Os direitos são aplicados a um documento estático? Se um ficheiro for enviado e os direitos necessitarem de ser alterados posteriormente, isto pode ser efectuado com a licença de publicação incorporada no ficheiro e não no servidor de "políticas" do RMS?

Sim, isto é possível quando utilizar o modelo de políticas do RMS: Quando o conteúdo é publicado com um modelo de políticas do RMS, a definição da política permanece no servidor e pode ser alterada por um administrador depois de o conteúdo ser publicado. Quando um utilizador requer uma licença para o conteúdo, a licença concederá direitos de acordo com a política actual definida no servidor. Se os direitos forem alterados após a emissão de uma licença de utilização para um utilizador, o utilizador continuará a ter os direitos em vigor no momento em que a licença de utilização foi emitida. Para aplicar um novo modelo de políticas de direitos depois da publicação do conteúdo, active uma política de expiração para o modelo e especifique a opção **As licenças de utilização de conteúdo devem ser renovadas a cada: n dias**. Em n, especifique o número de dias a partir dos quais um utilizador deverá requerer uma nova licença de utilização.
