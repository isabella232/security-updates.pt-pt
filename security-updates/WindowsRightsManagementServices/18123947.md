---
TOCTitle: Utilizar um Servidor do RMS
Title: Utilizar um Servidor do RMS
ms:assetid: '1533426b-89c2-43e0-8068-ca97ddab8606'
ms:contentKeyID: 18123947
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720205(v=WS.10)'
---

Utilizar um Servidor do RMS
===========================

A utilização de um servidor do RMS implica a gestão de tarefas executadas após a implementação do RMS numa organização. Esta secção inclui informações que o ajudam a gerir o servidor do RMS, procedimentos para tarefas de administração comuns, recursos para obtenção de informações adicionais e procedimentos recomendados.

Neste tema

-   [Gerir o RMS](https://technet.microsoft.com/9b573c55-c14c-436c-b3c5-7ba445de1562)
-   [RMS - Como ...](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)
-   [Recursos do RMS](https://technet.microsoft.com/d91221cf-e38e-4add-b7b9-50e63aad9a28)

Terminologia Utilizada neste Manual
-----------------------------------

**certificação de contas**  
Processo que associa as contas dos utilizadores aos pares de chaves no certificado de conta de direitos ou RAC.

<!-- -->

**serviço de certificação de contas**  
Serviço Web do RMS que cria e distribui certificados de contas de direitos. Consulte também certificação de conta.

<!-- -->

**serviço de proxy de activação**  
Serviço Web do RMS que suporta a activação do computador do cliente do RMS da versão 1.0. Utilizado para reencaminhar pedidos de activação de computadores para o Serviço de Activação da Microsoft. O serviço de activação gera um cofre exclusivo e um certificado de computador de RMS correspondente para o computador cliente, que o serviço proxy de activação do servidor do RMS reencaminha para o cliente requerente. Consulte também cofre.

<!-- -->

**serviço de administração**  
Serviço Web do RMS que hospeda o Web site de administração, permite gerir o RMS e actualiza a base de dados de configuração para o cluster.

<!-- -->

**manifesto de aplicação**  
Documento XML que descreve os módulos de uma aplicação associada activada por RMS e o que pode ser executado no ambiente da aplicação. Qualquer aplicação que escreva nas APIs do cliente do RMS para criar ou consumir informações protegidas pelo RMS deverá fornecer um manifesto em tempo de execução.

<!-- -->

**atributo**  
Propriedade de um objecto no Active Directory. Para cada classe de objectos, o esquema define os atributos que uma instância da classe deverá ter e os atributos adicionais que poderá ter.

<!-- -->

**associação**  
O mecanismo que exerce os direitos num sistema do RMS, em que o cliente do RMS valida as condições de uma licença de utilização em relação aos direitos que estão a ser pedidos. Se estas condições forem cumpridas, os direitos são concedidos.

<!-- -->

**certificado**  
Documento digital utilizado geralmente para autenticação e segurança de informações em redes abertas. Um certificado associa de forma segura uma chave pública à entidade que detém a chave privada correspondente. Os certificados são assinados digitalmente pela autoridade de certificação (AC) emissora, podendo ser emitidos para um utilizador, computador ou serviço. Consulte também chave privada; chave pública.

<!-- -->

**inscrição de clientes**  
O processo de criação do certificado de licenciador de clientes, o qual permite ao computador ou dispositivo do utilizador criar licenças de publicação que serão respeitadas por um servidor de licenciamentos.

<!-- -->

**certificado de licenciador de clientes**  
Certificado criado por um servidor do RMS e colocado em computadores cliente do RMS, que permite aos utilizadores publicarem conteúdo protegido offline sem estarem ligados à rede activada pelo RMS. O certificado de licenciador de clientes contém a chave que o cliente do RMS utiliza para assinar as licenças de publicação digitalmente.

<!-- -->

**condição**  
Conjunto de restrições e parâmetros especificados que fazem parte do grupo de direitos associado a uma licença de publicação. Estes entram em vigor no momento do consumo. Uma condição de tempo é uma condição comum que permite a um utilizador definir uma data de expiração para informações protegidas pelo RMS.

<!-- -->

**certificado de licenciador de clientes**  
Base de dados com informações de configuração do RMS para um servidor ou cluster.

<!-- -->

**consumo de conteúdo**  
Desencriptar e exercer os direitos de utilização numa peça de conteúdo protegido.

<!-- -->

**chave de conteúdo**  
A chave utilizada para encriptar e desencriptar conteúdo protegido durante a publicação e o consumo. Também conhecida como chave simétrica. O RMS utiliza chaves de conteúdo AES de 128 bits.

<!-- -->

**proprietário do conteúdo**  
Pessoa ou organização que estabelece a política de acesso ao conteúdo protegido.

<!-- -->

**desencriptação**  
Processo que tornar os dados encriptados novamente legíveis através da conversão do texto cifrado em texto normal.

<!-- -->

**assinatura digital**  
Meio utilizado pelos criadores de uma mensagem, ficheiro ou outras informações codificadas digitalmente para associarem a sua identidade às informações. O processo de assinatura digital das informações implica a transformação das informações, assim como de algumas informações secretas do remetente, num código denominado assinatura. As assinaturas digitais são utilizadas em ambientes de chaves públicas, fornecendo serviços de integridade e não rejeição.

<!-- -->

**serviço DRMRemote**  
Serviço Web do RMS que expõe serviços através do .NET Remoting, que é utilizado na comunicação entre diferentes servidores do RMS.

<!-- -->

**encriptação**  
Processo de conversão de informações num formulário que só pode ser lido por um destinatário específico. A encriptação é uma forma eficaz de manter as informações seguras. Para decifrar um ficheiro encriptado, o destinatário deverá ter a chave secreta ou a palavra-passe que o traduza. Consulte também encriptação de chave pública.

<!-- -->

**inscrição**  
Processo através do qual o servidor de certificações de raiz obtém um certificado de licenciador de servidores assinado pelo serviço de inscrição da Microsoft.

<!-- -->

**pedido de inscrição**  
Pedido enviado pelo servidor de certificação de raiz do RMS ao Serviço de Inscrição da Microsoft para obtenção de um certificado de licenciador de servidor.

<!-- -->

**exclusão**  
Processo utilizado pelo servidor do RMS para rejeitar um pedido de licença de utilização a um cliente baseado na política de exclusão. Consulte também lista de exclusões.

<!-- -->

**lista de exclusões**  
Lista de principais a que serão negadas licenças pelo serviço de licenciamento do RMS.

<!-- -->

**política de exclusão**  
Definições da base de dados de configuração do RMS que controlam a forma como a exclusão é aplicada na organização.

<!-- -->

**eXtensible rights Markup Language**  
Formato baseado em XML e utilizado pelo RMS para todas as licenças suportadas: certificados de computador, RACs, CLCs, licenças de utilização, licenças de publicação e certificados de licenciador de servidores que são documentos que especificam a política do RMS aplicada ao conteúdo protegido.

<!-- -->

**licença de emissão**  
Dados que especificam a política do RMS aplicada ao conteúdo protegido.

<!-- -->

**cluster de licenciamento**  
Um ou mais servidores que executam os serviços de publicação e licenciamento do RMS fora do cluster de certificações de raiz. Os servidores utilizam um URL de ligação e uma base de dados comum, e devem ser protegidos por um software ou um balanceador de carga de hardware se utilizar mais de um servidor. Ao contrário de um cluster de raiz ou certificação, os servidores do RMS num cluster de licenciamento não podem efectuar a certificação de utilizadores.

<!-- -->

**servidor de licenciamento**  
Servidor que executa os serviços de publicação e licenciamento do RMS fora do cluster de certificações de raiz.

<!-- -->

**serviço de licenciamento**  
Serviço Web do RMS que emite licenças de utilização.

<!-- -->

**cofre**  
Módulo de software responsável pela autenticação da utilização válida do conteúdo protegido, encriptação e desencriptação de informações e pela protecção do processamento de software fidedigno contra modificações e observações. Também conhecido como repositório seguro.

<!-- -->

**serviço de registo**  
Serviço de escuta do RMS que transfere dados registados da fila de mensagens para a base de dados de registo do servidor ou cluster do RMS.

<!-- -->

**activação de máquina**  
Processo de obtenção de um cofre e de um certificado de computador exclusivos para um computador na versão 1.0 do RMS. No RMS versão 1.0 SP1, a activação de computador é o processo de obtenção de um certificado de computador para cada utilizador desse computador.

<!-- -->

**manifesto**  
Um documento XML que descreve os módulos de uma aplicação associada, activada pelo RM, e o que pode ser executado no ambiente dessa aplicação.

<!-- -->

**Serviço de Activação da Microsoft**  
Serviço Web alojado pela Microsoft que emite certificados de computadores do RMS e cofres para pedidos de clientes do RMS da versão 1.0.

<!-- -->

**Serviço de Inscrição da Microsoft**  
Serviço Web alojado pela Microsoft que emite um certificado de licenciador de servidor para o servidor de certificações de raiz numa implementação do RMS.

<!-- -->

**pré-certificação**  
Funcionalidade do serviço de certificação do RMS que permite a um servidor do RMS pedir um certificado de conta de direitos em nome de um utilizador. Os certificados de contas de direitos obtidos com a pré-certificação só contêm a chave pública do utilizador.

<!-- -->

**principal**  
Entidade (como um utilizador, grupo ou gestor de conteúdo protegido) que desempenha uma função específica no esquema de segurança do RMS e na qual os objectos podem ser protegidos.

<!-- -->

**chave privada**  
A metade secreta de um par de chaves criptográficas utilizada com um algoritmo de chave pública. As chaves privadas são geralmente utilizadas para desencriptar uma chave de sessão simétrica, dados com assinatura digital ou dados que tenham sido encriptados com a chave pública correspondente. Consulte também chave pública; encriptação de chave pública.

<!-- -->

**aprovisionar**  
Para configurar um servidor do RMS para trabalhar numa organização.

<!-- -->

**chave pública**  
A metade não secreta de um par de chaves criptográficas utilizada com um algoritmo de chave pública. As chaves públicas são geralmente utilizadas quando encriptar uma chave de sessão, verificar uma assinatura digital ou encriptar dados que podem ser desencriptados com a chave privada correspondente. Consulte também chave privada; encriptação de chave pública.

<!-- -->

**encriptação de chave pública**  
Método de encriptação que utiliza duas chaves de encriptação relacionadas matematicamente. Uma chave chama-se chave privada e é confidencial. A outra chama-se chave pública e é fornecida livremente a todos os potenciais correspondentes. Num cenário típico, um remetente utiliza a chave pública do destinatário para encriptar uma mensagem. Apenas o destinatário tem a chave privada associada para desencriptar a mensagem. A complexidade da relação entre a chave pública e a chave privada significa que, desde que as chaves sejam suficientemente longas, é computacionalmente inviável distinguir uma da outra. Também chamada encriptação assimétrica. Consulte também chave privada; chave pública.

<!-- -->

**licença de publicação**  
A licença criada quando publicar conteúdo protegido pelo RMS. Entre outros itens, especifica quem pode aceder ao conteúdo, que direitos são concedidos e em que condições podem ser acedidos. Também conhecida como uma licença de emissão.

<!-- -->

**serviço de publicação**  
Serviço do RMS que assina as licenças de publicação e emite os certificados de licenciador de clientes. Consulte também certificado de licenciador de clientes; licença de publicação.

<!-- -->

**RAC**  
Consulte a definição de certificado de conta de direitos.

<!-- -->

**rights\_policy\_template\_gls**  
Um processo através do qual são listadas as entidades que não possuem licenças válidas.

<!-- -->

**lista de revogações**  
Documento baseado em XrML que lista os certificados e as licenças revogados pelo emissor. Consulte também revogação.

<!-- -->

**direito**  
Acção permitida aos utilizadores especificados para o conteúdo protegido pela tecnologia RMS. Esses direitos podem ser mais ou menos restringidos através de condições.

<!-- -->

**certificado de conta de direitos (RAC)**  
O certificado que utiliza o certificado do computador da activação do RMS para associar a conta e a chave de um utilizador a um computador específico ou grupos de computadores. Os componentes do certificado são utilizados para que os consumidores possam utilizar conteúdo protegido. Também conhecido como certificado de identidade de grupo (GIC) no RMS SDK.

<!-- -->

**RM (Gestão de Direitos)**  
Uma tecnologia que proporciona uma protecção contínua a dados digitais, utilizando encriptação, certificados e autenticação. Os destinatários ou utilizadores autorizados devem adquirir uma licença para poderem consumir os ficheiros protegidos de acordo com os direitos ou as regras negociais definidas pelo proprietário do conteúdo.

<!-- -->

**Cliente dos Serviços de Gestão de Direitos**  
Conjunto de APIs do RMS que cada computador cliente de um sistema RMS deve instalar. É um pré-requisito para a activação do computador, sendo necessário para a utilização das aplicações activadas pelo RMS.

<!-- -->

**modelo de política de direitos**  
Descreve um conjunto padrão de utilizadores, direitos e condições que podem ser aplicados ao conteúdo protegido pelo RMS. Quando um utilizador aplica um modelo de política de direitos a uma peça de conteúdo, as condições e os direitos nele descritos passam a fazer parte da licença de publicação.

<!-- -->

**Activação do RMS**  
Processo de colocação de um cofre no computador de um utilizador final no RMS versão 1.0. Isto só pode ser fornecido pelo serviço de activação do RMS, sendo essencial para a utilização da tecnologia RMS. No RMS versão 1.0 com o SP1, é o processo de obtenção de um certificado do computador para um utilizador desse computador e não requer uma ligação ao serviço de activação do RMS. Também conhecido como activação.

<!-- -->

**Serviço de Certificação do RMS**  
Serviço Web alojado pela Microsoft que emite certificados de contas de direitos para utilizadores com base nas respectivas credenciais do Microsoft .NET Passport.

<!-- -->

**Cliente de RMS**  
Conjunto de APIs do RMS que cada computador cliente de um sistema RMS deve instalar. É um pré-requisito para a activação do computador, sendo necessário para a utilização das aplicações activadas pelo RMS.

<!-- -->

**Certificado de computador do RMS**  
Certificado colocado no computador de um utilizador final durante a activação do RMS. A chave pública deste certificado é utilizada para encriptar a chave privada do utilizador contida nos certificados de contas de direitos do utilizador.

<!-- -->

**Aplicação activada pelo RMS**  
Aplicação expandida com o RMS SDK para permitir aos utilizadores especificarem os direitos anexados ao conteúdo criado.

<!-- -->

**Computador activado por RMS**  
Computador com o componente do cliente do RMS instalado e a activação do computador do RMS efectuada para que possa processar o conteúdo protegido pelo RMS.

<!-- -->

**Conteúdo protegido pelo RMS**  
Informações digitais protegidas pela tecnologia RMS.

<!-- -->

**cluster de certificações de raiz**  
Um ou mais servidores numa implementação do RMS que executam serviços de administração, inscrição, certificação de contas, proxy de activação, licenciamento e publicação. Esses servidores utilizam uma base de dados e um URL de ligação comum, e devem ser protegidos por um software ou um balanceador de carga de hardware. Só pode existir um cluster de certificações de raiz por cada floresta de Active Directory.

<!-- -->

**servidor de certificações de raiz**  
Servidor primário numa implementação do RMS que executa serviços de administração, inscrição, certificação de contas, proxy de activação, licenciamento e publicação. Só pode existir um servidor de certificações de raiz por cada floresta de Active Directory.

<!-- -->

**raiz de confiança**  
Entidade fidedigna que fornece a base para estabelecer a fidedignidade dos outros certificados. Todos os fornecedores de certificados e o utilizador final têm de confiar na raiz.

<!-- -->

**ID de segurança (SID)**  
Uma estrutura de dados do Windows que identifica cada utilizador, grupo e contas de computador do Windows. É emitido um SID exclusivo para cada conta da rede quando a conta é criada. Os processos internos do Windows referem-se ao SID de uma conta em vez de se referirem ao utilizador da conta ou ao nome do grupo.

<!-- -->

**certificado de licenciador de servidores**  
O certificado que estabelece as credenciais do servidor do RMS, facultando-lhe um serviço de licenciamento e de certificação válidos e permitindo a sua execução. O certificado de licenciador contém a chave pública utilizada para encriptar as chaves do conteúdo nas licenças de publicação.

<!-- -->

**serviço de servidor**  
Serviço Web do RMS destinado a ser utilizado por outro serviço.

<!-- -->

**SCP (ponto de ligação do serviço)**  
Objecto do Active Directory que referencia o URL do cluster de certificações de raiz de uma implementação do RMS. O cliente do RMS utiliza estas informações para localizar os serviços do RMS.

<!-- -->

**pré-inscrição**  
Um serviço Web do Windows RMS que permite a outro serviço pedir um certificado de licenciador de servidores e o URL da localização do serviço.

<!-- -->

**pedido de pré-inscrição**  
Um pedido enviado por um servidor de licenciamentos ao cluster de certificações de raiz a fim de obter um certificado de licenciador de servidores.

<!-- -->

**serviço de pré-inscrição**  
Serviço Web do RMS do servidor de certificações de raiz que responde aos pedidos de certificados de licenciadores de servidores submetidos pelos servidores de licenciamento durante o aprovisionamento.

<!-- -->

**super utilizador**  
Um membro do grupo de super utilizadores.

<!-- -->

**grupo de super utilizadores**  
Grupo de utilizadores opcional definido administrativamente para cada cluster do RMS e ao qual o servidor do RMS concede licenças de proprietários quando o conteúdo publicado por esse servidor for aberto.

<!-- -->

**licença de utilização**  
A licença que lista os direitos e as condições em que um utilizador final pode consumir o conteúdo protegido. Também conhecido por licença de utilizador final (EUL).
