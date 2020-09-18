## Pantalla de detalles del dispositivo {#pantalla-de-detalles-del-dispositivo}

Al hacer clic sobre cualquiera de los dispositivos listados en **Inicio &gt; Inventario &gt; Dispositivos**, al lado derecho de la pantalla visualizará el botón **Ver detalles**, el cual conduce a la pantalla de detalles del dispositivo.

Allí aparecerán las siguientes diez pestañas:

### General {#general}

Al hacer clic en la pestaña **General** encontrará las siguientes secciones:

#### Estado del Hardware {#estado-del-hardware}

En esta pestaña usted podrá realizar la consulta del estado en el que se encuentran los discos y la memoria del dispositivo.

#### Comandos de inicio {#comandos-de-inicio}

Al hacer clic en la pestaña **Comandos de Inicio**, se debe visualizar la información de las aplicaciones que inician con Windows.

#### Usuarios y grupos locales {#usuarios-y-grupos-locales}

Esta pantalla le proporcionará la información relacionada con los usuarios y grupos previamente creados.

### Hardware {#hardware}

Presenta el detalle de cada uno de los componentes físicos del dispositivo.

### Software {#software}

Aquí se visualizan los detalles del software del dispositivo clasificado en los siguientes 4 grupos:

#### **Software inventariado** {#software-inventariado}

#### **Actualizaciones** pendientes {#actualizaciones-pendientes}

#### Uso de software {#uso-de-software}

Aquí podrá visualizar distintos datos sobre el uso de software por parte de los usuarios, como las fechas y el tiempo de uso, versión de software, equipo desde el que se usó y quién lo usó. Estos datos pueden ser exportados en un archivo de Excel.

Se puede acceder a este módulo por dos rutas:

1.  **Software &gt; Catálogo** (seleccione el software cuyo uso desee ver) **&gt; Ver detalles &gt; Uso de Software**

Aquí puede escoger de la columna de la derecha los campos de las filas y las columnas para visualizar el uso del software seleccionado.

1.  **Inventario &gt; Dispositivos** (seleccione el dispositivo del que desee ver el uso que da al software) **&gt; Ver detalles &gt; Software &gt; Uso de Software**

Aquí puede escoger de la columna de la derecha los campos de las filas y las columnas para visualizar el uso de software en el dispositivo seleccionado.

Adicionalmente este módulo permite generar una gráfica con los datos filtrados. Esta gráfica se puede exportar como una imagen .png y puede ser del tipo:

*   Pie
*   Pie 3D
*   Doughnut
*   Doughnut 3D

#### Detalle de uso de software {#detalle-de-uso-de-software}

Aquí encontrará información detallada del uso del software.

### Administración remota {#administraci-n-remota}

La pestaña de administración remota está compuesta por los siguientes ocho módulos que permiten obtener información en línea.

#### Actividades {#actividades}

Aquí puede visualizar todo el historial de acciones de la consola ADM sobre el dispositivo.

#### Procesos {#procesos}

Aquí se encuentra el listado de procesos del dispositivo, adicionalmente se encuentra el PID, el uso en porcentaje de CPU y de memoria. Al hacer clic en el icono se finalizará la ejecución del proceso en el dispositivo.

#### Servicios {#servicios}

Aquí se encuentra el listado de todos los servicios que se encuentran en la consola de servicios de Windows (cmd- services.msc), al realizar alguna acción sobre los servicios, esta se verá reflejada en ADM y en la consola de servicios de Microsoft.

Para detener el servicio, haga clic en el icono

Se visualizará un mensaje informando que la acción fue ejecutada correctamente.

Para iniciar el servicio, haga clic sobre el icono

Se visualizará un mensaje en la parte inferior informando que la acción fue ejecutada correctamente.

Para pausar el servicio, haga clic sobre el icono

Se visualizará un mensaje en la parte inferior informando que la acción fue ejecutada correctamente.

Para reiniciar el servicio, haga clic sobre el icono

Se visualizará un mensaje en la parte inferior informando que la acción fue ejecutada correctamente.

#### Sesiones {#sesiones}

Aquí se visualizan todas las sesiones que están iniciadas en el dispositivo. Puede finalizar una sesión haciendo clic en el icono a la derecha.

**Nota:** Al cerrar una sesión de un usuario es posible que no se haya guardado toda la información de las aplicaciones, lo que puede conllevar a una pérdida de información.

Aparecerá un mensaje de confirmación verificando si realmente desea cerrar la sesión.

#### Archivos {#archivos}

Aquí se pueden visualizar todos los archivos del dispositivo. Puede eliminar un archivo haciendo clic en el icono .

Se visualizará un mensaje para confirmar que está seguro de eliminar el archivo, haga clic en **Aceptar**.

Finalmente, visualizará un mensaje de confirmación.

#### Llaves de registro {#llaves-de-registro}

Aquí se visualizan todas las llaves de registro que se encuentran en el editor de registro de Windows. Desde la consola es posible eliminar carpetas y llaves de registro, así como también crear claves, valor de cadena, valor de cadena expandible, valor Dword (32 Bits) y valor Qword (64 Bits).

**Nota:** El uso inadecuado de esta funcionalidad puede ocasionar mal funcionamiento o falla del dispositivo.

#### Conexiones {#conexiones}

Aquí se visualizan todas las peticiones que realiza el dispositivo, las respuestas a las peticiones, el protocolo de acceso, la dirección local, el puerto, la dirección externa y el estado.

#### Puntos de Restauración {#puntos-de-restauraci-n}

Esta función nos permite restaurar los archivos del sistema de alguno de los dispositivos a un estado anterior, incluyendo el sistema operativo y las aplicaciones instaladas.

Podemos usar esta función ante un cambio involuntario que se haya podido realizar y que altere el funcionamiento habitual del dispositivo.

Los puntos de restauración son una copia exacta del sistema operativo para algunas de las distribuciones de Windows; tenga en cuenta que para las distribuciones de Windows Server está disponible Windows Server Backup, la cual le proporciona un conjunto de asistentes y otras herramientas para realizar tareas básicas de copia y recuperación para el servidor. Las siguientes son las distribuciones con las cuales es posible usar esta funcionalidad:

| **Plataforma** | **Si** | **No** |
| --- | --- | --- |
| Windows 7 | X |  |
| Windows Vista | X |  |
| Windows 8 | X |  |
| Windows 8.1 | X |  |
| Windows 10 | X |  |
| Windows Server 2008 |  | X |
| Windows Server 2012 R2 |  | X |

**NOTA**: Si la máquina a la que se le aplicó un punto de restauración pertenece a un dominio, existe la posibilidad de que esta haya sido desasociada. Por lo anterior, se recomienda realizar nuevamente el proceso de integración de la máquina al dominio.

### Virtualización {#virtualizaci-n}

**Esta sección solo es visible en el detalle de los dispositivos que son virtualizadores.

Mediante la funcionalidad de virtualización, ADM incluye en el inventario los dispositivos virtualizados, y los hipervisores donde estos se encuentran alojados para tecnologías de virtualización de _Hyper-V_ de Microsoft. Aquí es posible realizar algunas tareas de administración de los ambientes virtuales.

**Nota**: Aranda Device Management soporta Hyper-V versión 2012 a 2016.

Para ir a esta función haga clic en **Inicio** **&gt; Inventario &gt;** **Dispositivos**, luego, en el costado izquierdo seleccione el filtro de **Virtualización** y haga clic en **Aplicar** **filtros**.

Luego haga clic en el botón **Ver detalles** y aparecerá la pestaña de **Virtualización**.

#### Configuración del acceso a las máquinas virtuales {#configuraci-n-del-acceso-a-las-m-quinas-virtuales}

En la pestaña de **Virtualización** podrá seleccionar la credencial con la que se va a acceder al dispositivo que contiene el hipervisor o crear una nueva haciendo clic en **Crear credencial**.

Tenga presente que el dispositivo debe estar en estado **En línea**.

**NOTA:** La credencial debe estar vinculada al grupo Administradores o Administradores de Hyper-V en la ventana **Administración de equipos** del dispositivo.

![C:\Users\ivonne.gonzalez\AppData\Local\Microsoft\Windows\INetCache\Content.Word\ADMMANUAL_152.png](C:\Users\jaime.chavarriaga\Documents\Test\export\assets\cusersivonnegonzalezappdatalo.png)

#### Gestión de máquinas virtuales {#gesti-n-de-m-quinas-virtuales}

En la pestaña **Virtualización**, podrá realizar la gestión de las máquinas virtuales configuradas en el dispositivo seleccionado.

Al hacer clic sobre la máquina virtual, se visualizará toda la información relacionada con la misma.

Haciendo clic sobre él ícono de la máquina virtual, se mostrarán las acciones que se pueden realizar sobre la maquina:

*   Encender
*   Desconectar
*   Suspender
*   Reiniciar
*   Apagar

### CI (Visualización) {#ci-visualizaci-n}

En esta pestaña podemos cargar la información de los CI (Configuration Items) a la CMDB. Un CI se refiere a cualquier componente o dispositivo que deba ser administrado para asegurar la prestación del servicio.

#### CI de un dispositivo {#ci-de-un-dispositivo}

Al seleccionar la pestaña **CI** en los detalles del dispositivo aparecerá la información del mismo; si no se tiene ningún campo mapeado, aparecerá una marca de agua indicando que no hay campos de CI configurados. Haga clic sobre **Actualizar CI** para traer la información actualizada de los campos de CI del dispositivo previamente configurados en la CMDB.

Aparecerá la siguiente ventana para confirmar la acción:

Al hacer clic en **Aceptar** se traerá la información actualizada y aparecerá un mensaje de proceso exitoso cuando la consulta se ha hecho correctamente.

#### CI de un software {#ci-de-un-software}

La información de un software aparecerá ingresando por **Inicio** **&gt; Software &gt;** **Catálogo** (seleccione el software deseado) **&gt; Ver detalles &gt; CI**.

Si no hay ningún campo mapeado, aparecerá una marca de agua indicando que se deben configurar los campos de mapeo o que se debe actualizar el CI para traer la información actualizada.

Al hacer clic sobre **Actualizar** **CI** aparecerá la siguiente ventana para confirmar la acción:

Al hacer clic en **Aceptar** aparecerá la información actualizada de los campos CI del software previamente configurados en la CMDB. Aparecerá un mensaje de proceso exitoso cuando la consulta se ha hecho correctamente.

Cuando se han creado licencias asociadas al software, estas aparecerán relacionadas dentro del CI del software como una tarjeta adicional con la información del mapeo de los campos de licencias.

### Información Adicional {#informaci-n-adicional}

En la pestaña de información adicional se almacena la información anexa que se considera relevante para la administración de los dispositivos. En caso de no tener información almacenada, se visualiza una marca de agua indicando que no hay información adicional, junto con el botón **Crear campos adicionales**.

El botón **Crear campos adicionales** lo direccionará a la pantalla de creación de campos adicionales a la cual también se puede llegar por **Configuración &gt; ADM &gt; Campos adicionales**. Allí podrá elegir de la lista en la esquina inferior izquierda el dispositivo al que le desea crear ese campo adicional, las opciones son: **Estación**, **Portatil**, **Servidor**, **Impresora**, **Switch** y **Router**. Luego haga clic en **Nuevo campo adicional**.

Aparecerá la siguiente pantalla:

Diligencie los campos **Etiqueta del campo adicional, Texto descriptivo, Texto de ayuda (Opcional)** y **Tipo de campo** en el cual están las siguientes opciones:

| **Tipo de campo** | **Descripción** |
| --- | --- |
| Texto corto | Cadena de texto corto con longitud máxima de 55 caracteres |
| Entero | Valor numérico |
| Fecha completa | Fecha en formato dd/MM/yyyy HH:mm |
| Hora | Hora en formato HH:mm |
| Fecha | Fecha en formato dd/MM/yyyy |
| Lista de opciones | Despliega un listado de opciones con selección de una única opción |
| Texto largo | Bloque de texto con longitud máxima de 255 caracteres |
| Booleano | Estados activo/inactivo |
| Decimal | Valor numérico con separador de decimales |
| Vínculo | Enlace de navegación |

Después de diligenciar estos campos haga clic en el botón **Agregar**. Encontrará que el campo adicional ha sido creado de la siguiente manera:

Haga clic en **Guardar** para completar exitosamente la creación del campo adicional.

La información aquí almacenada no tiene límite en la cantidad de campos a diligenciar.

**NOTA:** El diligenciamiento de la información adicional se hace por dispositivo y de forma manual.

Podrá acceder al campo adicional creado y diligenciarlo, siguiendo la ruta **Inicio &gt; Inventario &gt;** **Dispositivos** (seleccione el dispositivo en el que se creó el campo adicional) **&gt;** **Ver detalles &gt; Información adicional**.

Allí encontrará el campo adicional creado exitosamente. Diligencie el campo y haga clic en **Guardar**.

### Monitoreo {#monitoreo}

Esta función permite ver, en tiempo real, el porcentaje de uso del disco, de la memoria y del procesador de un dispositivo.

Se pueden crear diferentes tipos de monitoreo tipo Windows para cargar información de importancia en cada uno de los monitores que desee incluir en la aplicación, así:

**NOTA**: Actualmente la función de monitoreo no es soportada por SO de Windows 7.

#### Creación de un monitor {#creaci-n-de-un-monitor}

Para crear un monitor, haga clic en el botón **Agregar Monitor**.

Al ingresar, diligencie los campos **Nombre del monitor** y **Tipo del monitor**. Escoja si desea realizar el monitoreo por nombre del dispositivo o por dirección IP. Seleccione el intervalo de polling (sondeos), el tiempo de timeout (expiración) y las métricas que desea visualizar, las opciones son:

*   Porcentaje de uso de disco
*   Porcentaje de uso de memoria
*   Porcentaje de uso del procesador

Luego seleccione o agregue credenciales y haga clic en **Guarda**r.

**Nota:** Cuando se ingresen las credenciales de un usuario perteneciente a un dispositivo que no se encuentra en el dominio, se debe agregar **.\** y posteriormente el nombre del usuario, ej: .\Administrador.

Después de un tiempo prudente de recopilación de información de las métricas, la información se verá representada gráficamente de la siguiente manera (dependiendo de la actividad de la máquina monitoreada):

*   Porcentaje de uso del disco
*   Porcentaje de uso de memoria
*   Porcentaje de uso del procesador

**NOTAS**:

*   Solo es posible realizar la creación de un monitor según su tipo.
*   La información visualizada pertenece a la última hora de actividad

#### Pausar un monitor {#pausar-un-monitor}

Para pausar la representación gráfica de información, basta con ubicar el puntero sobre el tablero que se desea pausar y hacer clic sobre el ícono .

Si desea reanudar la representación gráfica de información, ubique el puntero sobre el tablero y haga clic en el ícono , se actualizará la información desde el momento en que fue pausada.

**NOTA:** La opción de pausa tiene como objetivo detener la gráfica visualmente más no impedir la recolección de información. Al realizar el cambio de pestaña, la gráfica volverá a su estado original, mostrando toda la información recolectada (incluyendo la información durante el tiempo de pausa).

#### Modificar la información de un monitor {#modificar-la-informaci-n-de-un-monitor}

Seleccione el monitor que desea editar y haga clic en el icono para editar.

Realice los cambios necesarios y posteriormente guarde la información.

Aparecerá un mensaje confirmando la modificación correcta.

#### Eliminar un monitor {#eliminar-un-monitor}

Seleccione el monitor a eliminar y haga clic en el ícono .

### Ubicación (Device Location) {#ubicaci-n-device-location}

Aquí podrá ver la localización geográfica del dispositivo gracias a una función de posicionamiento global del sistema operativo, de tal manera que se puede identificar el sitio exacto donde se encuentra el equipo y visualizarlo a través de un mapa.

**NOTA**: Aplica para versiones de Windows desde 8.1 en adelante y Mac OS. No aplica para servidores.

La ubicación geográfica del equipo se muestra a través de **OpenStreetMap**.

**NOTA:** La geolocalización presenta de 0 a 2 km de diferencia con la ubicación real. Esto se debe a que los dispositivos con la funcionalidad de ubicación o wifi desactivada presentan un nivel de frecuencia menor. Si desea tener una ubicación más acertada active la ubicación y el wifi en el dispositivo.

### Registro de fallos {#registro-de-fallos}

ADM versión 9.5 permite visualizar y gestionar fácilmente los potenciales problemas de identificación que ocurren con los dispositivos. Estos problemas se conocen como **conflictos** y se muestran en la sección de detalles de los dispositivos para que el usuario tome una decisión sobre cada uno de ellos. Así se logra evitar inconsistencias como la suplantación de máquinas y la duplicidad de registros.

La suplantación ocurre cuando varios dispositivos se ven como uno solo en la consola, como efecto principalmente de la clonación de equipos que ya tienen instalado el agente.

La duplicidad se presenta cuando una máquina tiene más de un registro asociado en la consola, normalmente debido al ingreso de máquinas que fueron formateadas después de tener el agente instalado.

Todo agente instalado en un dispositivo registra periódicamente con su servidor tres valores: una marca de hardware, la identificación asignada por el servidor y un token dinámico. Si alguno de estos valores no coincide con el que el servidor espera, se bloquean permanentemente las solicitudes de este equipo y se muestra un conflicto en la hoja de vida respectiva en la consola.

El usuario debe entonces resolver el conflicto eligiendo una acción cuando la solicitud de registro sospechosa vuelva a presentarse. El conflicto quedará resuelto cuando se presente la siguiente solicitud.

Todos los dispositivos que presenten conflictos de identificación serán marcados con el icono y podrán filtrarse en el listado para que el usuario pueda gestionarlas fácilmente.

![C:\Users\ivonne.gonzalez\AppData\Local\Microsoft\Windows\INetCache\Content.Word\800px-ADM_E_Conflicts001.png](C:\Users\jaime.chavarriaga\Documents\Test\export\assets\cusersivonnegonzalezappdatalo.png)

Al entrar a la sección de detalles del dispositivo, en la pestaña **Registro de fallos**,aparecerá una lista con todos los conflictos detectados para el dispositivo.

En cada caso se indica el tipo de conflicto y se habilita un selector para la acción a tomar. Los conflictos pueden ser de dos tipos: **hardware duplicado** o **identificador duplicado**. Puede hacer clic en el icono en la parte superior derecha para abrir el panel de ayuda donde se explica cada uno de ellos y cómo deben resolverse.

Las posibles acciones a tomar son: asociar dispositivo, crear dispositivo o dejar la acción pendiente. El usuario podría también borrar el conflicto si considera que ya no volverá a ocurrir.

Es posible que el usuario sepa de antemano que un tipo específico de conflicto se presentará muy frecuentemente para un dispositivo. Por ejemplo, si una máquina virtual fue clonada muchas veces después de tener el agente instalado y se pretenden ingresar todos los clones al sistema (generando conflictos de identificador duplicado), o si una máquina física es formateada y reingresada cada semana para ser usada en campañas diferentes (generando conflictos de hardware duplicado). En estos casos los conflictos son predecibles y el usuario puede configurar una acción automática.

![C:\Users\ivonne.gonzalez\AppData\Local\Microsoft\Windows\INetCache\Content.Word\800px-ADM_E_Conflicts004.png](C:\Users\jaime.chavarriaga\Documents\Test\export\assets\cusersivonnegonzalezappdatalo.png)