---
title: Obtención y procesamiento de inventarios
chapter: "inventarios"
---

La información de cada dispositivo se obtiene de varias maneras:

*   Al momento del descubrimiento a través de protocolos _agent-less,_ como SNMP y WMI, se captura información básica del dispositivo como el tipo, el sistema operativo y la IP.
*   Cuando el agente se instala por primera vez, se envía un inventario resumido, que contiene información más completa, pero sin un nivel alto de detalle.
*   Cuando el agente está instalado y ya envió su primer inventario, se continúa con inventarios de alto nivel de detalle y de todos los tipos.

Los inventarios se transmiten como paquetes de datos entre los agentes instalados en los dispositivos gestionados y el servidor. El servidor procesa estos inventarios tomando acciones automáticas de acuerdo a diferentes valores y a las reglas de negocio ingresadas por el usuario; además, alimenta el histórico visible de eventos para cada máquina.

Los paquetes de inventarios de ADM viajan cifrados, facilitando la prevención de fuga de datos (DLP). Cada módulo tiene su propio tipo de inventarios, por lo tanto, tenemos inventarios de activos, parches, métricas de uso, archivos y energía. Los paquetes generados en los agentes se guardan temporalmente en carpetas locales del dispositivo hasta que puedan ser enviados a su respectivo _conserver_.

Los paquetes en algunas ocasiones son fraccionados y generados de manera incremental por parte del agente para evitar una alta ocupación de red con paquetes muy grandes. Los tamaños mínimos de un inventario son de menos de 1 KB. Los tamaños máximos están en la siguiente tabla:

**Tamaño máximo de inventarios**

| | |
| :--- | :-- |
| **HW/SW** | 100 kb |
| **Archivos totales** | 1 MB |
| **Incrementales** | 12 kb |
| **Parches y actualizaciones** | 4 kb |
| **Energía** | 1 kb |
| **Uso** | 10 kb |

Los valores de la tabla anterior deben tenerse en cuenta para el cálculo del ancho de banda consumido por la solución.

**Registro periódico de agentes: **El consumo de ancho de banda también se afecta por el hecho de que los agentes realizan la operación de registro cada cinco minutos (esto es configurable). Dicho registro consiste en una llamada al servidor, pasando por los conservers respectivos, para actualizar la información de identificación. El primer registro de un agente lleva información básica de inventario y pesa alrededor de 1.5 KB. De ahí en adelante cada registro pesa aproximadamente 0.25 KB.
