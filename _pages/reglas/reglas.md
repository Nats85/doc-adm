---
title: Reglas
chapter: "reglas"
---

El módulo de reglas se utiliza para automatizar el proceso de actualización de parches. Por medio de este proceso es posible programar la descarga de actualizaciones, programar el envío de ejecuciones, notificar alertas o enviar notificaciones por correo. Estas acciones se ejecutan siempre que las condiciones de la regla se cumplan.

Para configurar una regla, diríjase a **Inicio &gt; Reglas**:

Allí despliegue la lista **Más opciones**, bajo el título **Nueva** r**egla** visualizará los tres tipos de regla que puede crear: Actualizaciones, Descubrimiento y Dispositivos,

### Actualizaciones {#actualizaciones}

Aquí se configuran las reglas que se aplican después de realizar un inventario de actualizaciones (parches). Elija la posición **Activo** en el botón de **Estado** e ingrese el nombre de la regla.

![800px-ADMMANUAL_03200](C:\Users\jaime.chavarriaga\Documents\Test\export\assets\800px-admmanual03200.png)

Luego ingrese las condiciones de la regla.

![800px-ADMMANUAL_02800](C:\Users\jaime.chavarriaga\Documents\Test\export\assets\800px-admmanual02800.png)

Finalmente ingrese el tipo de acción que desea realizar y haga clic en **Guardar**.

![800px-ADMMANUAL_02900](C:\Users\jaime.chavarriaga\Documents\Test\export\assets\800px-admmanual02900.png)

La nueva regla se visualizará en la pantalla de reglas.

### Descubrimiento {#descubrimiento}

Aquí se configuran las reglas que se evalúan después de realizar un descubrimiento de dispositivos. Elija la posición **Activo** en el botón de **Estado** e ingrese el nombre de la regla.

Luego ingrese las condiciones de la regla.

Finalmente ingrese el tipo de acción que desea realizar y haga clic en **Guardar**.

La nueva regla se visualizará en la pantalla de reglas.

### Dispositivos {#dispositivos}

Aquí se configuran las reglas que se evalúan después de realizar un inventario de HW/SW. Elija la posición **Activo** en el botón de **Estado** e ingrese el nombre de la regla.

Diligenciar la información básica de la regla.

Luego ingrese las condiciones de la regla.

Finalmente ingrese el tipo de acción que desea realizar y haga clic en **Guardar**.

La nueva regla se visualizará en la pantalla de reglas.

**Nota para reglas de dispositivos:** en caso de que haya eliminado el dispositivo del grupo, al ejecutar la regla por segunda vez no se devolverá el dispositivo al grupo, a menos que la regla obtenga una actualización o se reinicie el servicio Windows de &quot;ArandaCrucherInventory&quot;.

![ArandaCruncherInventory](C:\Users\jaime.chavarriaga\Documents\Test\export\assets\arandacruncherinventory.png)
