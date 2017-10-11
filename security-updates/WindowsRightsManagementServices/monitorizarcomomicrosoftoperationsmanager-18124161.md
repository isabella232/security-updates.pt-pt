---
TOCTitle: Monitorizar com o Microsoft Operations Manager
Title: Monitorizar com o Microsoft Operations Manager
ms:assetid: 'ce372598-7421-4f1f-b8eb-f62da26e85d1'
ms:contentKeyID: 18124161
ms:mtpsurl: 'https://technet.microsoft.com/pt-pt/library/Cc747758(v=WS.10)'
---

Monitorizar com o Microsoft Operations Manager
==============================================

O RMS inclui um pacote de gestão que pode utilizar com o Microsoft® Operations Manager (MOM). Pode utilizar o MOM para gerir as operações dos servidores existentes na organização, nomeadamente a:

-   Controlar eventos colocados no registo de eventos da aplicação pelo RMS.
-   Realçar eventos que possam indicar possíveis falhas de serviço ou problemas na configuração, o que lhe permite tomar imediatamente medidas de correcção ou prevenção.
-   Emitir alertas para avisos e erros, tais como o da expiração do certificado de licenciador de servidores ou a falha de um serviço Web.

O RMS Management Pack (RMS\_MOMPack.akm) é instalado com o RMS na pasta %programfiles%\\Windows Rights Management Services\\Tools.

Este pacote de gestão contém os seguintes conjuntos de regras, que podem ser utilizados para ajudar o administrador do RMS a gerir a implementação do servidor do RMS.

**Regras do RMS MOM Management Pack**

1.  PMC Measure - Activation Proxy total failures
2.  PMC Measure - Activation Proxy Total time
3.  PMC Measure - Activation Total Processing Time
4.  PMC Measure - Activation Total Reqs
5.  PMC Measure - ActivationProxy total reqs
6.  PMC Measure - AD cache (DB cache) hits
7.  PMC Measure - AD cache (DB cache) misses
8.  PMC Measure - Average License Processing time
9.  Event - Configuration Info corruption
10. PMC Measure - Dead GC connections
11. PMC Measure - Enroll failures
12. Event - General Error
13. Event - Init Failure
14. Event - Licensor Cert has expired
15. Event - Licensor Cert Request Failure
16. Event - Logging service failure
17. PMC Measure - Max GC connections available
18. Event - Missing License Acq Point generation plugin
19. PMC Measure - MSMQ Queue length on all RM servers
20. Event - No GCs available
21. Event - Plugin Init Failure
22. Event - PrivateKey protection password changed
23. Event - RM Server Shut Down
24. Event - RM Server ShutDown Failure
25. Event - Server Startup Failure
26. PMC Measure - SubEnroll failures
27. Event - SuperUser privileged override power was invoked
28. PMC Threshold - Too Many GetLicensorCert failures
29. Event - Upcoming Licensor Cert Expiry - 1 Month
30. Event - Upcoming Licensor Cert expiry - 1 Week

Para mais informações sobre como implementar os pacotes de gestão MOM na organização, consulte o [Web site da Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).
