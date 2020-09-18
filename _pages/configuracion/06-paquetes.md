---
title: Paquetes
chapter: "configuracion"
---

Este módulo permite cargar ejecutables con extensiones BAT, MSI, MSU y EXE, creando paquetes útiles en los proyectos de distribución de agente y software; teniendo en cuenta que estos tienen una única configuración de arquitectura y sistema operativo.

### Creación de paquetes de software {#creaci-n-de-paquetes-de-software}

Para configurar paquetes de agente, ingrese a **Configuración &gt; ADM &gt; Paquetes**, despliegue la lista **Más opciones** y seleccione la opción **Paquete**.

**NOTA**: Ingrese la línea de comandos que se debe usar en el momento de la ejecución de la instalación, por ejemplo, se deberá incluir siempre la opción de instalación silenciosa para que en el momento de la ejecución no solicite ninguna información al usuario.

Diligencie la información del formulario según el tipo de sistema operativo:

#### Windows {#windows}

1.  Seleccione el tipo de paquete: Software.
2.  Tipo de sistema operativo: Windows.
3.  Seleccione la arquitectura: Puede ser 32 bits (x86), 64 bits (x64) o ambas.
4.  Ingrese el nombre del paquete.
5.  Ingrese la versión.
6.  Ingrese una breve descripción.
7.  Seleccione el archivo.

#### Linux {#linux}

1.  Seleccione el tipo de paquete: Software.
2.  Tipo de sistema operativo: Linux.
3.  Seleccione la arquitectura: Puede ser 32 bits (x86), 64 bits (x64) o ambas.
4.  Ingrese el nombre del paquete.
5.  Ingrese la versión.
6.  Ingrese una breve descripción.
7.  Seleccione el archivo.

#### Mac {#mac}

1.  Seleccione el tipo de paquete: Software.
2.  Tipo de sistema operativo: Linux.
3.  Seleccione la arquitectura: Puede ser 32 bits (x86), 64 bits (x64) o ambas.
4.  Ingrese el nombre del paquete.
5.  Ingrese la versión.
6.  Ingrese una breve descripción.
7.  Seleccione el archivo.

### Creación de paquetes de agente {#creaci-n-de-paquetes-de-agente}

Para configurar paquetes de agente, ingrese a **Configuración &gt; ADM &gt; Paquetes**, despliegue la lista **Más opciones** y seleccione la opción **Paquete**:

#### Windows {#windows-0}

Seleccione el agente para tipo de sistema operativo **Windows**, una vez seleccionado el archivo, la información del formulario se diligenciará automáticamente. Si desea puede ingresar una breve descripción del paquete.

#### Linux {#linux-0}

Seleccione el agente para el tipo de sistema operativo **Linux**, una vez seleccionado el archivo, la información del formulario se diligenciará automáticamente. Si desea puede ingresar una breve descripción del paquete.

**Nota:** El agente no es soportado para distribuciones Linux de 32 bits

#### Mac {#mac-0}

Seleccione el agente para el tipo de sistema operativo **Mac**, una vez seleccionado el archivo, la información del formulario se diligenciará automáticamente. Si desea puede ingresar una breve descripción del paquete.
