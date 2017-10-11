---
TOCTitle: 'FAQ sobre o RMS: Administração'
Title: 'FAQ sobre o RMS: Administração'
ms:assetid: '43f77336-5e62-4405-9efb-55417a402d62'
ms:contentKeyID: 18123962
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747547(v=WS.10)'
---

FAQ sobre o RMS: Administração
==============================

Perguntas Mais Frequentes Sobre a Administração do RMS
------------------------------------------------------

-   [Qual é a melhor forma de revogar as permissões sobre os documentos para um utilizador que sai de uma organização?](#bkmk_1)
-   [Quando estabelecer políticas de fidedignidade entre duas organizações para trocar conteúdo do RMS, o certificado de licença XrML emitido para a empresa confiante necessita de um processamento especial?](#bkmk_2)
-   [Como funciona o RMS com perfis de utilizadores itinerantes?](#bkmk_3)
-   [Por que motivo quereria uma organização desactivar o RMS?](#bkmk_4)
-   [Qual é o processo de desactivação geral?](#bkmk_5)
-   [É possível desactivar um servidor do RMS para que apenas alguns utilizadores consigam recuperar documentos?](#bkmk_6)
-   [Qual é o significado de o servidor não conseguir aceder ao directório da aplicação?](#bkmk_7)
-   [É possível usar o rastreio no servidor do RMS?](#bkmk_8)
-   [Qual é o desfasamento de relógio e como é possível resolver a situação?](#bkmk_9)

<span id="BKMK_1"></span>
#### Qual é a melhor forma de revogar as permissões sobre os documentos para um utilizador que sai de uma organização?

Em geral, é melhor ter documentos licenciados para grupos de utilizadores definidos no Active Directory em vez de contas de utilizadores individuais. Isto é recomendado para que, quando um utilizador sai de uma organização, seja possível remover o utilizador do grupo do Active Directory e o utilizador não consiga ler documentos enviados para esse grupo. No entanto, o utilizador ainda pode ler os documentos com licenças de utilização existentes, excepto se os documentos tiverem os direitos definidos para requerer ao utilizador uma licença de utilizador sempre que o documento for aberto. Se este direito não estiver definido, a única forma de impedir o utilizador de abrir documentos com licenças de utilização existentes é eliminando a licença de utilizador guardada no computador do utilizador.

<span id="BKMK_2"></span>
#### Quando estabelecer políticas de fidedignidade entre duas organizações para trocar conteúdo do RMS, o certificado de licença XrML emitido para a empresa confiante necessita de um processamento especial?

Quando estabelecer um domínio de utilizadores fidedignos ou um domínio de publicação fidedigno, está a considerar a organização do parceiro fidedigna para participar no sistema de gestão de direitos. Como tal, está a considerar, mediante um risco calculado, que a confiança na outra organização não compromete as suas informações. Como procedimento recomendado, peça à organização do parceiro que envie o seu certificado de servidor licenciador do RMS através de um canal autenticado, como correio electrónico S/MIME, para ajudar a atenuar o risco de danificar o certificado de servidor licenciador antes de o importar para o seu servidor do RMS.

<span id="BKMK_3"></span>
#### Como funciona o RMS com perfis de utilizadores itinerantes?

Os certificados de contas de direitos (RACs) utilizados para identificar os utilizadores são específicos para os computadores. Quando utilizar perfis itinerantes, a primeira utilização do RMS num determinado computador criará um novo RAC para o utilizador nesse computador.

<span id="BKMK_4"></span>
#### Por que motivo quereria uma organização desactivar o RMS?

A desactivação do RMS remove o servidor do RMS da infra-estrutura e fornece uma forma para os utilizadores guardarem conteúdo protegido por direitos sem protecção. Existem três razões principais para que as organizações optem por este procedimento:

-   Simplificar o projecto de arquitectura, como a consolidação de servidores num cluster.
-   Migrar um ambiente piloto de prova de conceito para um ambiente de produção.
-   Intercalar servidores do RMS após uma aquisição.

<span id="BKMK_5"></span>
#### Qual é o processo de desactivação geral?

O processo de desactivação é iniciado a partir do cluster de raiz do RMS através da activação do serviço de desactivação. Quando o serviço de desactivação for activado, todos os outros serviços (por exemplo, licenciamento e certificação) são desactivados. Em seguida, é necessário direccionar a aplicação activada pelo RMS do utilizador para se ligar ao serviço de desactivação quando uma funcionalidade do RMS é utilizada. O Microsoft Office 2003 é um exemplo de uma aplicação activada pelo RMS. No Office 2003, o cliente do RMS é direccionado através de chaves de registo. Uma chave de registo específica identifica o serviço de desactivação. Assim que esta chave for configurada para direccionar o cliente para o serviço de desactivação, o cluster do RMS concederá licenças de utilização com permissões completas (leitura, escrita, cópia, impressão, edição, etc.) ao utilizador para esse conteúdo, independentemente de essas permissões terem sido atribuídas originalmente ao utilizador ou não. Os utilizadores devem ser direccionados para remover todas as protecções de direitos de quaisquer documentos que queiram reter depois de o cluster do RMS ser completamente desactivado. Assim que este procedimento estiver concluído, o cluster do RMS pode ser retirado completamente de serviço.

Como procedimento recomendado, efectue uma cópia de segurança da base de dados de configuração do cluster do RMS, em caso de precisar de recuperar um documento protegido por direitos após a retirada do cluster. Sem a chave privada do cluster de raiz do RMS, apenas o autor do documento conseguirá abrir o conteúdo protegido por direitos após a retirada do servidor.

<span id="BKMK_6"></span>
#### É possível desactivar um servidor do RMS para que apenas alguns utilizadores consigam recuperar documentos?

Pode aplicar uma lista de controlo de acesso (ACL) ao serviço de desactivação Web (decommission.asmx) para controlar o acesso ao serviço de desactivação, de modo a que apenas determinados utilizadores consigam obter a chave de desencriptação para o conteúdo protegido por direitos.

<span id="BKMK_7"></span>
#### Qual é o significado de o servidor não conseguir aceder ao directório da aplicação?

Por vezes, este erro aparece quando tenta abrir o Web site de administração do RMS pela primeira vez após a instalação do RMS. Depois de receber esta mensagem de erro, não é possível configurar ou administrar o RMS.

Este erro ocorre geralmente quando os Serviços de Informação Internet (IIS) estão a ser executados no modo de isolamento IIS 5.0. Utilize o procedimento seguinte para desactivar esta definição no servidor e reinicie o IIS para resolver este problema.

**Para desactivar o modo de isolamento do IIS 5.0**
1.  Inicie sessão no servidor do RMS como membro do grupo de Administradores local.

2.  Clique em **Iniciar**, aponte para **Ferramentas Administrativas** e, em seguida, clique em **Gestor dos Serviços de Informação Internet (IIS)**.

3.  No **Gestor de IIS**, expanda o computador local, clique com o botão direito do rato em **Web Sites** e, em seguida, clique em **Propriedades**.

4.  Clique no separador **Serviço**, desmarque a caixa de verificação **Executar serviço WWW no modo de isolamento do IIS 5.0** e, em seguida, clique em **OK**.

5.  Esta alteração requer que o serviço IIS seja reiniciado. Quando lhe for pedido para reiniciar o serviço IIS, clique em **Sim**.

<span id="BKMK_8"></span>
#### É possível usar o rastreio no servidor do RMS?

Como os Serviços de Gestão de Direitos foram criados com o Microsoft® .NET Framework, é possível activar o rastreio para ajudar a acompanhar eventos do sistema e a resolver problemas.

Pode implementar o rastreio se modificar o ficheiro Web.config ou Machine.config. Quando implementar o rastreio no ficheiro Machine.config, este é efectuado em todos os componentes de software que estejam no computador; no entanto, se implementar o rastreio no ficheiro Web.config, apenas os eventos que ocorram nos serviços Web são rastreados.

**Para activar o rastreio**
1.  Abra o ficheiro Machine.config ou Web.config e, em seguida, adicione as linhas seguintes na secção &lt;system.diagnostics&gt; que está no ficheiro:

    
        ```
2.  Reinicie o IIS executando o IISRESET a partir de uma linha de comandos.

3.  Depois de recolher todos os dados necessários, remova do ficheiro .config as linhas que foram adicionadas no passo 1.

4.  Reinicie o IIS executando o IISRESET a partir de uma linha de comandos.

| ![](images/Cc747547.Important(WS.10).gif)Importante                                                                                                                                                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Quando utilizar o rastreio num servidor do RMS, podem ocorrer problemas de desempenho, como atrasos maiores nas aquisições de licenças de utilização e emissão de certificados de contas de direitos. Utilize apenas o rastreio em circunstâncias limitadas para o ajudar a diagnosticar e a resolver problemas existentes. |

<span id="BKMK_9"></span>
#### Qual é o desfasamento de relógio e como é possível resolver a situação?

O desfasamento de relógio dá-se quando a hora do relógio de um computador difere da hora do relógio de outro computador. Esta ocorrência é bastante comum, sendo tão comum como os relógios de pulso de duas pessoas que se encontram na mesma sala apresentarem horas ligeiramente diferentes. O desfasamento de relógio pode causar problemas sempre que especificar o prazo de validade de uma licença.

A hora de validade de uma licença é definida de acordo com o relógio do fabricante. O desfasamento de relógio pode causar problemas em dois locais do ciclo de publicação e de consumo:

-   Quando uma aplicação tentar adquirir uma licença de utilização através da licença de publicação com uma hora de validade passada ou futura, de acordo com o relógio do servidor do RMS. Neste caso, o pedido falha. Isto pode ocorrer com um utilizador final quando requerer uma licença de utilização, ou com uma aplicação que esteja a tentar pré-licenciar um documento (para adquirir uma licença de utilização em nome de um utilizador).
-   Se a hora de validade da licença tiver expirado (ou ainda nem tiver começado), a tentativa de utilização da licença falhará. Caso contrário, apenas estarão indisponíveis os direitos expirados (ou que ainda não sejam válidos).

Por exemplo, se o relógio de um computador de publicação estiver 15 minutos atrasado em relação ao relógio de um computador de consumo, e o fabricante criar uma licença de publicação que especifique que o conteúdo expira em 15 minutos, o consumidor receberia uma licença de utilização inutilizável do servidor porque os direitos de visualização do conteúdo concedidos pela licença de utilização já teriam expirado.

Não existe qualquer solução perfeita para os problemas de desfasamento de relógio. Uma boa solução é a definição da hora de validade de início de um direito antes da hora actual para os consumidores com relógios atrasados e, se possível, ampliar a hora de validade da licença para os utilizadores com relógios adiantados. Recomenda-se que não se esqueça do impacto dos problemas do desfasamento de relógio, especialmente quando criar licenças com prazos de validade curtos.
