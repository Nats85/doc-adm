---
title: Software
chapter: "software"
---

### Configuración

En el menú **Inicio &gt; Software &gt; Distribución** despliegue el menú de **Más opciones** y seleccione **Software**. Tenga en cuenta que previamente debe estar configurado el contenedor de archivos (Ver [7.2.4 Catálogo de aplicaciones](..\configuracion\catalogo_de_aplicaciones.md))

Ingrese la información del formulario, seleccione el tipo de sistema operativo sobre el que va a realizar la distribución, seleccione el paquete a instalar y haga clic en **Guardar**.

**NOTA:** El paquete de software debe estar previamente creado y configurado (ver [7.2.5.1 Creación de paquetes de software](..\configuracion\paquetes.md#creaci-n-de-paquetes-de-software)).

### Acciones

Una vez configurado el proyecto, se mostrará el botón **Ver detalles**. Luego de entrar a la pantalla de detalles del proyecto, encontrará al costado izquierdo las acciones disponibles para realizar, a saber:

#### Ejecutar proyecto

Esta acción se emplea para ejecutar el proyecto de distribución de software.

Se visualizará la pantalla en la que se debe establecer la configuración de la ejecución y los dispositivos a los que desea realizar la distribución del software.

En la pestaña **Configuración**, ingrese la información del nombre que recibirá la ejecución, el tipo de ejecución, la programación de notificaciones y las credenciales (en caso de no haber configurado previamente la credencial de ejecución haga clic en el botón **Crear credencial**).

En la pestaña **Dispositivos**, seleccione los dispositivos sobre los cuales desea realizar la distribución.

Tan pronto finalice la configuración, guarde los cambios realizados. En el panel izquierdo se mostrará la ejecución creada y la información de la configuración realizada.

Una vez completada la instalación, el progreso de la ejecución cambia a Ejecutado.

La ejecución del proyecto tiene disponible cuatro acciones ubicadas en la parte superior derecha de la pestaña **Actividad**:

*   **Actualizar**: Refresca la información del progreso de la ejecución sobre el o los dispositivos.
*   **Reintentar**: Intente nuevamente enviar la ejecución del proyecto sobre el o los dispositivos seleccionados.
*   **Detener**: Si la ejecución del proyecto está vigente, interrumpe el proceso de distribución.
*   **Eliminar**: Remueve del listado la ejecución seleccionada.

#### Editar Proyecto

Seleccionando esta opción usted podrá modificar la información suministrada en la creación del proyecto.

#### Eliminar proyecto

Al seleccionar esta opción usted podrá eliminar el proyecto del listado de distribución, junto con toda la información de las ejecuciones. Aparecerá una ventana con un mensaje solicitando confirmar la acción.
