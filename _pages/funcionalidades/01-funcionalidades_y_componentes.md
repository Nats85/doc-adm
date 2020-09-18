---
title: Funcionalidades y componentes
chapter: "funcionalidades"
---

![](/assets/componentes-adm.png)



El **Servidor de Aplicaciones** contiene los componentes que tienen acceso directo al **Servidor de base de datos**. Aquí se encuentran:

* **RepServer** \(receptor\) que se encarga de recibir las solicitudes provenientes de la red LAN del cliente.
* **Consola Web de ADM** que permite a los usuarios interactuar con los activos a gestionar.
* **Servicios** **Windows de procesamiento de inventarios** \(Crunchers\) que son los encargados de recolectar y organizar estructuradamente los inventarios recibidos por el RepServer. Estos son: ArandaCruncherEnergy, ArandaCruncherFile, ArandaCruncherInventory y ArandaCruncherPatch
* **Servicios Windows comunes de Aranda** que son: License, Mailer y Worker; estos controlan el licenciamiento de producto, el envío de emails y el procesamiento en segundo plano, respectivamente.

El **Conserver** \(servidor de comunicaciones\) actúa como enlace entre los componentes del servidor de aplicaciones y la red LAN del cliente. Este es un servicio Windows que debe estar ubicado en la red LAN para poder enviar y recibir mensajes de los agentes instalados en cada máquina, adicionalmente facilita los procesos de descubrimiento \(por IP, DNS, ICMP, Netbios, SNMP, SMB, WMI y Dominio\), distribución y administración remota. Dependiendo de la topología se deberá instalar un Conserver por cada segmento de red.

El **Agente** es un programa instalado en cada máquina gestionada que permite la generación de inventarios y la administración segura de comandos provenientes del servidor. Los agentes se comunican entre sí a través de P2P \(red entre pares\) para facilitar la distribución de archivos y para reducir sustancialmente la ocupación del canal de entrada de la red corporativa. Existe un agente para cada una de las plataformas soportadas. Los agentes normalmente son instalados en las máquinas a través de un proceso de distribución guiado desde la consola, sin embargo, existen múltiples alternativas de despliegue las cuales pueden combinarse para cubrir los diferentes escenarios de infraestructura. Al instalar el agente, se crea una serie de servicios en el dispositivo que permiten establecer la comunicación con el visor de control remoto y la gestión general del dispositivo.

El **Visor de Soporte Remoto** es un aplicativo que permite tomar control remoto de las máquinas gestionadas y debe estar instalado en la red LAN para que pueda acceder a ellas. Este visor debe tener también acceso al servidor de aplicaciones para poder autorizar y coordinar la sesión.
