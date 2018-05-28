---
TOCTitle: Activar o Serviço de Desactivação
Title: Activar o Serviço de Desactivação
ms:assetid: '45226e85-b50d-41cc-aca7-0f603f8509d5'
ms:contentKeyID: 18123965
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720261(v=WS.10)'
---

Activar o Serviço de Desactivação
=================================

A desactivação do sistema do RMS requer a chave privada utilizada para proteger todas as informações publicadas. Esta chave privada está armazenada na base de dados de configuração, é encriptada pela API de Protecção de Dados (DPAPI) e baseia-se na palavra-passe introduzida durante o aprovisionamento. Se a chave privada do RMS for guardada num módulo de segurança por hardware (HSM), a chave privada será guardada no HSM, em vez da base de dados de configuração.

| ![](/security-updates/images/Cc720261.Caution(WS.10).gif)Atenção                                                                                                                                     |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Antes de desactivar o sistema do RMS, certifique-se de que conhece a sua palavra-passe na chave privada. Se não conhecer esta palavra-passe, deve reiniciar a chave privada antes de desactivar o servidor RMS. |

O primeiro passo para remover o sistema RMS é desactivar os servidores no cluster. Uma vez que a desactivação constitui uma função de licenciamento, é possível desactivar um servidor num cluster de licenciamento pré-inscrito do RMS, sem afectar o cluster de raiz do RMS ou qualquer outro cluster de licenciamento pré-inscrito. Por essa razão, necessita de desactivar separadamente o cluster de raiz do RMS e quaisquer clusters de licenciamento, uma vez que cada cluster de licenciamento possui a sua própria chave privada para criar licenças de publicação.

Utilize o procedimento descrito a seguir para activar o serviço de desactivação:

1.  Abra o Web site Administração do Windows RMS.
2.  Clique em **Administrar o RMS** e, em seguida, clique em **Definições de Segurança**.
3.  Seleccione a caixa de verificação **Permitir a desactivação da instalação do RMS**.
4.  Quando uma caixa de diálogo solicitar a confirmação do processo de desactivação, clique em **OK**.

Quando desactiva um servidor, este não pode ser restaurado para uma configuração padrão do RMS. Este procedimento é irreversível.

Depois de desactivar o RMS, este deve ser completamente removido através de **Adicionar e Remover Programas** antes de tentar instalar outra versão do RMS.
