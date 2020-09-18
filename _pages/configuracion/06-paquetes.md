---
title: Paquetes
chapter: "configuracion"
---

Este módulo permite cargar ejecutables con extensiones BAT, MSI, MSU y EXE, creando paquetes útiles en los proyectos de distribución de agente y software; teniendo en cuenta que estos tienen una única configuración de arquitectura y sistema operativo.

### Creación de paquetes de software

Para configurar paquetes de agente, ingrese a **Configuración &gt; ADM &gt; Paquetes**, despliegue la lista **Más opciones** y seleccione la opción **Paquete**.

[]({{ site.baseurl }}/assets/images/paquetes_1.png)

**NOTA**: Ingrese la línea de comandos que se debe usar en el momento de la ejecución de la instalación, por ejemplo, se deberá incluir siempre la opción de instalación silenciosa para que en el momento de la ejecución no solicite ninguna información al usuario.

Diligencie la información del formulario según el tipo de sistema operativo:

#### Windows

1.  Seleccione el tipo de paquete: Software.
2.  Tipo de sistema operativo: Windows.
3.  Seleccione la arquitectura: Puede ser 32 bits (x86), 64 bits (x64) o ambas.
4.  Ingrese el nombre del paquete.
5.  Ingrese la versión.
6.  Ingrese una breve descripción.
7.  Seleccione el archivo.

[]({{ site.baseurl }}/assets/images/Windows_1.png)

#### Linux

1.  Seleccione el tipo de paquete: Software.
2.  Tipo de sistema operativo: Linux.
3.  Seleccione la arquitectura: Puede ser 32 bits (x86), 64 bits (x64) o ambas.
4.  Ingrese el nombre del paquete.
5.  Ingrese la versión.
6.  Ingrese una breve descripción.
7.  Seleccione el archivo.

[]({{ site.baseurl }}/assets/images/Linux_1.png)

#### Mac

1.  Seleccione el tipo de paquete: Software.
2.  Tipo de sistema operativo: Linux.
3.  Seleccione la arquitectura: Puede ser 32 bits (x86), 64 bits (x64) o ambas.
4.  Ingrese el nombre del paquete.
5.  Ingrese la versión.
6.  Ingrese una breve descripción.
7.  Seleccione el archivo.

[]({{ site.baseurl }}/assets/images/Mac_1.png)

### Creación de paquetes de agente

Para configurar paquetes de agente, ingrese a **Configuración &gt; ADM &gt; Paquetes**, despliegue la lista **Más opciones** y seleccione la opción **Paquete**:

[]({{ site.baseurl }}/assets/images/paq_1.png)

#### Windows

Seleccione el agente para tipo de sistema operativo **Windows**, una vez seleccionado el archivo, la información del formulario se diligenciará automáticamente. Si desea puede ingresar una breve descripción del paquete.

[]({{ site.baseurl }}/assets/images/paq_win_1.png)

#### Linux

Seleccione el agente para el tipo de sistema operativo **Linux**, una vez seleccionado el archivo, la información del formulario se diligenciará automáticamente. Si desea puede ingresar una breve descripción del paquete.

[]({{ site.baseurl }}/assets/images/paq_linux_1.png)

**Nota:** El agente no es soportado para distribuciones Linux de 32 bits

#### Mac

Seleccione el agente para el tipo de sistema operativo **Mac**, una vez seleccionado el archivo, la información del formulario se diligenciará automáticamente. Si desea puede ingresar una breve descripción del paquete.

[]({{ site.baseurl }}/assets/images/paq_mac_1.png)
