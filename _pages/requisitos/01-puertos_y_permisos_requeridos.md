---
title: Puertos utilizados por la aplicación
chapter: "requisitos"
---

Los siguientes son los puertos de comunicación usados por Aranda Device Management (ADM).
Es necesario configurar la red para permitir las comunicaciones a través de estos puertos.

| **Puerto** | **Protocolo** | **Origen** | **Destino** | **Dirección** | **Descripción** |
| :--- |  :--- | :--- | :--- | :--- | :--- |
| **80** | **TCP, UDP** | Agente, Conserver | Agente, Conserver | Bidireccional | Requerido para la conexión de los clientes con el servidor. |
| **9025** | **TCP, UDP** | Consolas Web, Conserver | Agente (todas las máquinas de la red) | Bidireccional | Requerido para la comunicación del servidor con el agente y para la administración remota. |
| **9125** | **TCP** | Consolas Web | Todas las máquinas de la red | Bidireccional | Requerido para el control remoto RFB. |
| **139** | **TCP** | Conserver | Todas las máquinas de la red | Bidireccional | Despliegue de Agentes |
| **445** | **TCP** | Conserver | Todas las máquinas de la red | Bidireccional | Despliegue de Agentes |
| **389** | **TCP, UDP** | Conserver | Controladores de Dominio | Bidireccional | Conexión LDAP |
| **1433** | **TCP** | Consolas Web, Repserver | Servidor de Base de Datos | Bidireccional | Servidor Base de Datos. Se puede modificar el puerto si se requiere, se deben habilitar los permisos sobre ese puerto. |
| **1884** | **TCP** | Agente, Conserver | Servidor de aplicaciones | Bidireccional | Requerido para la conexión de los clientes con el servidor. |
| **9501** | **TCP** | Conserver | Todas las máquinas de la red | Bidireccional | Comunicación entre agentes. |
