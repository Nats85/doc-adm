---
title: Comunicaciones
chapter: "configuracion"
---

### Repserver

Ingrese a **Configuración &gt; ADM &gt; Comunicaciones**, y visualizará un árbol cuyo nodo principal es el RepServer, este siempre será visible y solo debe existir uno en estado activo. La primera vez que se ingresa a la consola se debe configurar la dirección del nodo de comunicaciones. Para obtener la dirección del RepServer, ingrese al **IIS (Internet Information Services) &gt; Sitios &gt;Sitios por defecto &gt; Repserver**.

[]({{ site.baseurl }}/assets/images/repserver_1.png)

Al hacer clic en **Browse** (navegar) por el puerto, se abre un navegador con la URL de la aplicación web, en este caso la URL es [https://localhost/Repserver/](https://localhost/Repserver/), la sección de dominio &#039;localhost&#039; se debe reemplazar por la dirección IP del dispositivo o el nombre. Copie esta URL y péguela en el campo **Dirección nodo de comunicaciones**. En el campo **Almacenamiento de archivos**, ingrese la ruta donde van a permanecer los archivos temporalmente, luego haga clic en **Probar conexión** y **Guardar**. Al finalizar, se debe visualizar una pantalla informando que se encuentra en línea el Repserver.

[]({{ site.baseurl }}/assets/images/repserver_2.png)

### Comunicación de agente

En la pantalla Comunicaciones seleccione la pestaña **Comunicación de agente** del RepServer.

[]({{ site.baseurl }}/assets/images/comun_1.png)

#### Configuración global

En la sección de configuración global para las comunicaciones del agente se debe ingresar la información correspondiente a los intervalos de sincronización y el puerto designado.

[]({{ site.baseurl }}/assets/images/config_1.png)

#### Configuración P2P

Al activar esta característica se puede realizar la descarga de archivos a través de red P2P (Peer to Peer). Una vez activo se habilitarán los siguientes campos:

*   Puerto de descarga archivo P2P.
*   Retención de archivos.
*   Velocidad de descarga.
*   Velocidad de subida.

[]({{ site.baseurl }}/assets/images/P2P_1.png)

### Conserver

Al momento de instalar el Conserver todos los archivos permanecen en la ruta **C:\ Program Files (x86) \ Aranda \ Conserver**, allí se encuentra el archivo Aranda.Conserver.Windows.Service.exe.config el cual se debe configurar de la siguiente manera para que se comunique con el Repserver:

| **Configuración appSettings** |
| --- |
| **&lt;add key=&quot;serverAddress&quot; value=&quot;Dirección del Repserver/&quot;/&gt;** | Dirección donde se encuentra el Repserver |
| **&lt;add key=&quot;enableProxy&quot; value=&quot;false&quot;/&gt;** | En caso de usar Proxy se habilita la etiqueta enableProxy con valor &quot;true&quot; |
| **&lt;add key=&quot;proxyAddress&quot; value=&quot;&quot;/&gt;** | Dirección del proxy |
| **&lt;add key=&quot;proxyUser&quot; value=&quot;&quot;/&gt;** | Usuario del Proxy |
| **&lt;add key=&quot;proxyPassword&quot; value=&quot;&quot;/&gt;** | Password del proxy |
| **&lt;add key=&quot;logLevel&quot; value=&quot;Information&quot;/&gt;** | Nivel de verbosidad log del conserver; &quot;Information&quot;, &quot;Debug&quot;, &quot;Detailed&quot;, &quot;verbose&quot;. Por defecto se encuentra parametrizado &quot;Information&quot;. |
| **&lt;add key=&quot;privateIp&quot; value=&quot;Ip&quot;/&gt;** | Identificador en la red Interna del Conserver, debe ir la Ip. |
| **&lt;add key=&quot;publicIp&quot; value=&quot;Ip&quot;/&gt;** | Identificador de red del conserver desde el exterior, debe ir la Ip. (En Caso de que no se requiera se coloca la misma dirección Ip privada). |
| **&lt;add key=&quot;mqttServerPort&quot; value=&quot;1884&quot;/&gt;** | Puerto de Comunicación de mqtt, por defecto se encuentra parametrizado el &quot;1884&quot;. |
| **&lt;add key=&quot;mqttIp&quot; value=&quot;Ip&quot;/&gt;** | Identificador de Mqtt en la red Interna, debe ir la IP. |
| **&lt;add key=&quot;publicServerPort&quot; value=&quot;80&quot;/&gt;** | Puerto de Comunicación red pública de Conserver, por defecto se encuentra parametrizado el &quot;80&quot;. |
| **&lt;add key=&quot;privateServerPort&quot; value=&quot;80&quot;/&gt;** | Puerto de Comunicación red privada de Conserver, por defecto se encuentra parametrizado el &quot;80&quot;. |
| **&lt;add key=&quot;p2pPort&quot; value=&quot;9501&quot;/&gt;** | Puerto para conexiones p2p, por defecto se encuentra parametrizado el &quot;9501&quot;. |
| **&lt;add key=&quot;maxDistributionSleepMsPerThread&quot; value=&quot;8&quot;/&gt;** |  |
| **&lt;add key=&quot;maxDistributionThreads&quot; value=&quot;4&quot;/&gt;** | Estos dos últimos tag son utilizados para el funcionamiento interno del sistema, no se deben modificar. |

[]({{ site.baseurl }}/assets/images/conserver1.png)

Inicie el servicio Aranda Conserver Service, que permite la comunicación con el Repserver.

[]({{ site.baseurl }}/assets/images/conserver2.png)

En la consola Aranda Device Management, ingrese a **Configuración &gt; ADM &gt; Comunicaciones**, se visualizará el árbol de comunicaciones donde está el nodo del Repserver, al hacer clic sobre el nodo se despliegan todos los Conserver que se están comunicando.

[]({{ site.baseurl }}/assets/images/conserver3.png)

La primera vez que se visualiza el Conserver se debe realizar la configuración de los campos **Puerto Wake on LAN** y **Almacenamiento de archivos**. La configuración del puerto depende de la administración, pero normalmente es el número 7, la ruta de almacenamiento de archivos corresponde a la ubicación temporal de almacenamiento.

[]({{ site.baseurl }}/assets/images/conserver4.png)

### Descubrimiento de dispositivos

El descubrimiento de dispositivos se realiza solo la primera vez que se desea instalar el agente a un dispositivo, este se puede realizar por diferentes medios (IP, DNS, ICMP, NetBIOS SMB, WMI, Dominio). El siguiente es el paso a paso de la configuración del descubrimiento de dispositivos.

Ingrese a **Configuración &gt; ADM &gt; Comunicaciones**, seleccione el nodo del Conserver y haga clic en la pestaña Descubrimiento, visualizará el formulario para realizar el descubrimiento, ingrese la información solicitada.

[]({{ site.baseurl }}/assets/images/dispositivos1.png)

Ingrese la información en el programador para que se ejecute, de lo contrario no se realizará esta acción. Adicionalmente, ingrese la información de periodicidad para que se realice cada cierto tiempo, sin necesidad de configurar nuevamente.
