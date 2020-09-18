---
title: Instalación del Agente en Windows
chapter: "instalacion"
---

## Instalación usando el programa instalador

El tercer instalador es `Aranda.Agent.Windows.x86\_x64` y sirve para instalar los servicios requeridos para el Agente ADM en Windows.
Puede instalarse de manera desatendida y automática a través de la funcionalidad de distribución de agente de la consola Web de ADM, o de forma manual haciendo uso de la interfaz de usuario.

El siguiente es el paso a paso de la instalación manual del Agente: _**Hola como estas?**_

Haga clic sobre el instalador Aranda Agent.

![]({{ site.baseurl }}/assets/images/agen_1.png)

A continuación, visualizará un mensaje informando que se va a instalar Aranda Agent.

![]({{ site.baseurl }}/assets/images/agen_2.png)

Si tiene un archivo de configuración seleccione **Sí** e ingrese la ruta, de lo contrario, seleccione **No** y haga clic en **Siguiente**.

![]({{ site.baseurl }}/assets/images/agen_3.png)

Al ingresar 0 como identificador del perfil, significa que va a descargar el perfil que esté configurado por defecto; ingrese la dirección de Conserver \(se encuentra en el módulo

  **Configuración &gt; Aranda Device Management &gt; Comunicaciones &gt; Nodo del Conserver**\).

![]({{ site.baseurl }}/assets/images/agen_4.png)

Ingrese el nombre de usuario y la organización donde se instalará el agente.

![]({{ site.baseurl }}/assets/images/agen_5.png)

Seleccione el tipo de instalación que desea realizar \(completa o personalizada\) y haga clic en **Siguiente**.

![]({{ site.baseurl }}/assets/images/agen_6.png)

A continuación, iniciará la instalación del agente.

![]({{ site.baseurl }}/assets/images/agen_7.png)

Una vez finalizada la instalación del agente, haga clic en **Finalizar**

![]({{ site.baseurl }}/assets/images/agen_8.png)

## Instalación manual del Agente por línea de comandos en

Para realizar la instalación del Agente ADM por línea de comando se puede ejecutar la siguiente instrucción desde el _command promt_ de Windows:

```
Aranda.Agent.Windows.x86\_x64.9.3.1803.0108 /S /V"/norestart /qn AGENT\_SERVER\_ADDRESS=http://localhost/Conserver AGENT\_PROFILE\_ID=0"
```

| | |
| :-- | :-- |
| `AGENT\_PROFILE\_ID=\[UNIT\]` | Identificador del perfil a instalar, 0 es un perfil seleccionado en la aplicación como perfil por defecto. |
| `AGENT\_SERVER\_ADDRESS=\[STRING\]` | es la ruta de Conserver. |

## Instalación manual del Agente por línea de comandos en Linux y OSX {#instalaci-n-manual-del-agente-por-l-nea-de-comando-linux-macos}

Para realizar la instalación del Agente ADM por línea de comando se puede ejecutar la siguiente instrucción desde un intérprete de comandos de Linux o macOS

> **Nota:** El agente no es soportado para distribuciones Linux de 32 bits

```
sh RUTA\_INSTALADOR/Aranda.Agent.Linux.x64.9.3.1801.3001.sh -- AGENT\_SERVER\_ADDRESS=http://localhost/Conserver AGENT\_PROFILE\_ID=0
```

| | |
| :-- | :-- |
| `RUTA\_INSTALADOR=` | Ruta donde se encuentra el instalador, puede ser relativa o absoluta |
| `AGENT\_PROFILE\_ID=\[UNIT\]` | Identificador del perfil a instalar, 0 es un perfil seleccionado en la aplicación como perfil por defecto |
| `AGENT\_SERVER\_ADDRESS=\[STRING\]` | es la ruta de Conserver. |

### Actualización automática del Agente {#actualizaci-n-autom-tica-del-agente}

Para realizar la actualización automática del agente, ingrese a la consola Web de ADM y diríjase a **Configuración &gt; ADM &gt;** **Paquetes**.

Luego haga clic en **Más Opciones** y seleccione **Paquete**

Suba el paquete del agente a instalar

Después de transcurridas 8 horas el agente intenta actualizarse con la versión más reciente publicada en la consola.
