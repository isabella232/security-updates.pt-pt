---
TOCTitle: Configurar Dispositivos de Encriptação de Hardware
Title: Configurar Dispositivos de Encriptação de Hardware
ms:assetid: '3a35a8ea-696c-4005-9892-cac6e773497a'
ms:contentKeyID: 18123978
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc720248(v=WS.10)'
---

Configurar Dispositivos de Encriptação de Hardware
==================================================

O RMS pode utilizar fornecedores de serviços criptográficos (CSP) padrão da Microsoft, tais como CSPs básicos e avançados, para gerar as chaves pública e privada que serão armazenadas na base de dados de configuração e utilizadas para proteger o conteúdo. Recomenda-se que seja aplicada protecção adicional a estas chaves pois são armazenadas no software. Para fornecer protecção de chave de nível mais elevado, pode utilizar um CSP baseado em hardware disponibilizado por um módulo de segurança por hardware (HSM).

Se utilizar um HSM para fornecer segurança adicional às chaves dos servidores, instale e configure o hardware nos servidores antes de iniciar a instalação do RMS.
