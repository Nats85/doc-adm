---
title: Acciones
chapter: "inventario"
---

Las siguientes son las acciones disponibles para ejecutar sobre los dispositivos:

### Obtener inventario

El inventario se puede obtener de diferentes formas:

*   La primera vez que se instala el agente, se generan los diferentes inventarios, entre esos el de HW/SW.
*   Otra manera es desde la consola ADM, ingresando al menú **Inventario &gt; Dispositivos**. Allí debe seleccionar los dispositivos disponibles y luego hacer clic en la acción **Obtener inventario**.

![]({{ site.baseurl }}/assets/images/inv_1.png)

En la lista desplegable seleccione **HW/SW**.

![]({{ site.baseurl }}/assets/images/inv_2.png)

Es posible obtener el inventario inmediatamente o programarlo. El agente genera un archivo AAM que se encuentra cifrado.

El agente envía el archivo al Repserver, para que se procese y actualice la información en la base de datos; es posible verificar si se realizó la actualización, en la tarjeta del dispositivo pasados algunos minutos.

![]({{ site.baseurl }}/assets/images/inv_3.png)

### Actualización del CI

Al seleccionar la pestaña **CI** en la hoja de vida del dispositivo se cargará la información; en caso de no tener ningún campo mapeado, aparecerá una marca de agua indicando que se deben configurar los campos de mapeo o que se debe actualizar el CI para traer la información actualizada.

![]({{ site.baseurl }}/assets/images/CI_1.png)

Al hacer clic sobre la acción de actualizar CI se desplegarán los botones de confirmación.

![]({{ site.baseurl }}/assets/images/CI_2.png)

Al hacer clic sobre aceptar se traerá la información actualizada de los campos de CI del dispositivo previamente configurados en la CMDB. Aparecerá un mensaje de éxito cuando la consulta se ha hecho correctamente.

![]({{ site.baseurl }}/assets/images/CI_3.png)

### Control remoto

Para realizar control remoto se debe tener configurado previamente lo siguiente:

*   El perfil del agente debe tener activo el producto de control remoto (Ver:

    7.2.3\. Perfil Agente

    ).
*   Se debe instalar el componente Aranda.ADM.Utils.Installer.exe en el dispositivo (Ver: [5.4\. Instalación del visor de soporte remoto](..\instalacion\instalacion_del_visor_de_soporte_remoto.md))
*   Su dispositivo debe estar asociado a un grupo que contenga permisos para realizar control remoto. Para esto siga los siguientes pasos:

En **Configuración &gt; Generales &gt; Grupos** haga clic en el icono que aparece al lado del nombre del grupo al que desea otorgar permisos de control remoto. Luego haga clic en **Editar permisos para soporte remoto** al lado derecho de la pantalla.

![]({{ site.baseurl }}/assets/images/control_remoto_9.png)

Aparecerá una ventana en donde se pueden seleccionar grupos o usuarios (ubicándolos con la barra de búsqueda) y definir para cada uno el rol que tendrá sobre estas máquinas (Administrador/Gestor).

![]({{ site.baseurl }}/assets/images/control_remoto_10.png)

Finalizada esta acción, haga clic sobre el botón **Agregar Dispositivo** para agregar el dispositivo al cual se quiere acceder remotamente.

![]({{ site.baseurl }}/assets/images/control_remoto_11.png)

Busque el dispositivo y haga clic en **Agregar**.

![]({{ site.baseurl }}/assets/images/control_remoto_12.png)

Verifique que se haya agregado el dispositivo correctamente (en la parte inferior de la pantalla se muestra un mensaje de confirmación).

![]({{ site.baseurl }}/assets/images/control_remoto_13.png)

En caso de querer realizar control remoto omitiendo las autorizaciones debe seleccionar el campo **Omitir autorización** en la configuración de roles del grupo.

El rol &#039;Remote Support Administrator&#039; ya tiene seleccionada esta opción por defecto.

![]({{ site.baseurl }}/assets/images/control_remoto_14.png)

**NOTA:** Si el dispositivo de destino ya tiene una sesión iniciada por RPC (Remote Procedure Call), NO podrá realizar control remoto desde la consola de ADM a excepción de que tenga habilitado el campo &#039;Omitir autorizaciones&#039;.

Una vez realizada la configuración anterior, haga clic en **Control Remoto** del dispositivo seleccionado.

![]({{ site.baseurl }}/assets/images/control_remoto_15.png)

Haga clic en el botón **Aceptar**.

![]({{ site.baseurl }}/assets/images/control_remoto_16.png)

Se visualizará un mensaje solicitando abrir una URL para acceder al control remoto de la máquina.

![]({{ site.baseurl }}/assets/images/control_remoto_17.png)

Se mostrará una pantalla con la imagen del dispositivo a través de control remoto.

![]({{ site.baseurl }}/assets/images/control_remoto_18.png)

**NOTA**: En caso de requerir que no se soliciten las credenciales de autenticación para establecer una conexión de control remoto a un dispositivo, se debe agregar en la tabla &#039;AFW_SETTINGS&#039; de la base de datos la configuración que se muestra a continuación:

![]({{ site.baseurl }}/assets/images/control_remoto_19.png)

**Nota:** Actualmente el control remoto necesita de una confirmación para poder ejecutarse. En los navegadores que tengan habilitada la opción de &quot;Bloquear ventanas emergentes&quot; no se podrá visualizar el mensaje. Es necesario deshabilitar esa opción para poder ejecutar el visor de control remoto normalmente.

![]({{ site.baseurl }}/assets/images/control_remoto_20.png)

**NOTA** Al momento de hacer la grabación, la resolución quedará ajustada según el tamaño de la ventana del visor.

**NOTA:** Existe la opción de obtener un Log de &#039;Control remoto&#039;. En caso de querer obtenerlo debe realizar las siguientes configuraciones.

1.  Dentro de la carpeta de C:\ProgramFiles\Aranda\ADM Utils se encuentra un archivo con el nombre &quot;Aranda.AVS.Viewer.exe.Config&quot; abrirlo con algún editor de texto.
2.  En el archivo la linea: &quot;&lt;add key=&quot;logLevel&quot; value=&quot;Information&quot; /&gt;&quot; cambiar o modificar por &quot;&lt;add key=&quot;logLevel&quot; value=&quot;Debug&quot; /&gt;&quot;
3.  Ejecutar control remoto desde la consola de ADM. Inmediatamente se debe crear un archivo en la ruta:

C:\ProgramData\Aranda\Aranda.AVS.Viewer.Application\RemoteControl.log

### Distribuir Agente

Permite realizar la distribución de agentes para lo cual deberá seleccionar uno de los proyectos de distribución de software previamente creados en el módulo de distribución. Deberá definir si desea ejecutarlo inmediatamente o programarlo para una fecha futura y las credenciales de ejecución.

![]({{ site.baseurl }}/assets/images/distr_1.png)

### Distribuir proyecto

![]({{ site.baseurl }}/assets/images/distr_2.png)

Permite realizar la distribución de un proyecto de software previamente configurado al dispositivo seleccionado, haciendo uso de una contraseña para su ejecución. Deberá definir si desea ejecutarlo inmediatamente o programarlo para una fecha futura y las credenciales de ejecución.

![]({{ site.baseurl }}/assets/images/distr_3.png)

### Más acciones

![]({{ site.baseurl }}/assets/images/mas_1.png)

Permite acceder a un listado con las siguientes acciones adicionales para realizar sobre el dispositivo:

*   Ejecutar comando

Aquí podrá enviar líneas de comando a un dispositivo según el sistema operativo que este tenga (Linux, Mac o Windows).

![]({{ site.baseurl }}/assets/images/comando_1.png)

Deberá definir el usuario a nombre del cual se ejecutará dicho comando y si desea ejecutarlo inmediatamente o programarlo para una fecha futura.

![]({{ site.baseurl }}/assets/images/comando_2.png)

*   Eliminar dispositivos

Esta acción retira del inventario el dispositivo seleccionado y toda su información relacionada.

![]({{ site.baseurl }}/assets/images/eliminar_1.png)

*   Reiniciar dispositivo

Esta acción reinicia el dispositivo seleccionado. Puede ejecutar el reinicio inmediatamente o programarlo para una fecha futura.

![]({{ site.baseurl }}/assets/images/reiniciar_1.png)

*   Apagar dispositivo

Puede apagar el dispositivo inmediatamente o programarlo para una fecha futura.

![]({{ site.baseurl }}/assets/images/apagar_1.png)

**Nota:** Esta acción solo funciona en dispositivos con &quot;WakeOnLan&quot;.

*   Encender dispositivo

Esta acción se ejecuta inmediatamente.

![]({{ site.baseurl }}/assets/images/encender_1.png)

*   Sincronizar reloj

Esta acción se emplea para que el reloj del dispositivo seleccionado concuerde con el del servidor donde se instaló la consola ADM.

![]({{ site.baseurl }}/assets/images/sinc_1.png)

**Nota:** En el SO MAC se debe reiniciar el dispositivo para evidenciar el cambio.

*   Borrar archivos por extensión

Esta acción le permite eliminar todos los archivos que tengan una misma extensión dentro del dispositivo seleccionado. Es especialmente útil para borrar archivos malignos o liberar espacio eliminando masivamente archivos innecesarios. El borrado puede ejecutarse inmediatamente o programarse para una fecha futura.

![]({{ site.baseurl }}/assets/images/borrar_1.png)

*   Cambiar perfil del agente

Esta acción permite cambiar el perfil del agente instalado en el dispositivo por otro perfil de configuración que se haya creado previamente en la consola ADM.

![]({{ site.baseurl }}/assets/images/cambiar_perfil_1.png)

*   Enviar mensaje

Con esta acción podrá enviar mensajes a los dispositivos seleccionados. Es útil para notificar a los usuarios de los dispositivos acerca de algún evento como problemas operativos o cambios en la red o en el servidor.

![]({{ site.baseurl }}/assets/images/enviar_msj_1.png)

*   Asignar usuario responsable

Aquí podrá buscar y seleccionar al usuario que será responsable de los dispositivos seleccionados.

![]({{ site.baseurl }}/assets/images/asigar_1.png)

*   Resolver conflictos

Esta acción le permite resolver conflictos de hardware duplicado y de identificador duplicado en el dispositivo con dos soluciones posibles que deben aplicarse así:

![]({{ site.baseurl }}/assets/images/tabla10.png)
