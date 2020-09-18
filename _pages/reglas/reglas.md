---
title: Reglas
chapter: "reglas"
---

El módulo de reglas se utiliza para automatizar el proceso de actualización de parches. Por medio de este proceso es posible programar la descarga de actualizaciones, programar el envío de ejecuciones, notificar alertas o enviar notificaciones por correo. Estas acciones se ejecutan siempre que las condiciones de la regla se cumplan.

Para configurar una regla, diríjase a **Inicio &gt; Reglas**:

![]({{ site.baseurl }}/assets/images/rule_1.png)

Allí despliegue la lista **Más opciones**, bajo el título **Nueva** r**egla** visualizará los tres tipos de regla que puede crear: Actualizaciones, Descubrimiento y Dispositivos,

![]({{ site.baseurl }}/assets/images/rule_2.png)

### Actualizaciones

Aquí se configuran las reglas que se aplican después de realizar un inventario de actualizaciones (parches). Elija la posición **Activo** en el botón de **Estado** e ingrese el nombre de la regla.

![]({{ site.baseurl }}/assets/images/rule_3.png)

Luego ingrese las condiciones de la regla.

![]({{ site.baseurl }}/assets/images/rule_4.png)

Finalmente ingrese el tipo de acción que desea realizar y haga clic en **Guardar**.

![]({{ site.baseurl }}/assets/images/rule_5.png)

La nueva regla se visualizará en la pantalla de reglas.

### Descubrimiento

Aquí se configuran las reglas que se evalúan después de realizar un descubrimiento de dispositivos. Elija la posición **Activo** en el botón de **Estado** e ingrese el nombre de la regla.

![]({{ site.baseurl }}/assets/images/rule_6.png)

Luego ingrese las condiciones de la regla.

![]({{ site.baseurl }}/assets/images/rule_7.png)

Finalmente ingrese el tipo de acción que desea realizar y haga clic en **Guardar**.

![]({{ site.baseurl }}/assets/images/rule_8.png)

La nueva regla se visualizará en la pantalla de reglas.

![]({{ site.baseurl }}/assets/images/rule_9.png)

### Dispositivos

Aquí se configuran las reglas que se evalúan después de realizar un inventario de HW/SW. Elija la posición **Activo** en el botón de **Estado** e ingrese el nombre de la regla.

Diligenciar la información básica de la regla.

![]({{ site.baseurl }}/assets/images/rule_10.png)

Luego ingrese las condiciones de la regla.

![]({{ site.baseurl }}/assets/images/rule_11.png)

Finalmente ingrese el tipo de acción que desea realizar y haga clic en **Guardar**.

![]({{ site.baseurl }}/assets/images/rule_12.png)

La nueva regla se visualizará en la pantalla de reglas.

![]({{ site.baseurl }}/assets/images/rule_13.png)

**Nota para reglas de dispositivos:** en caso de que haya eliminado el dispositivo del grupo, al ejecutar la regla por segunda vez no se devolverá el dispositivo al grupo, a menos que la regla obtenga una actualización o se reinicie el servicio Windows de &quot;ArandaCrucherInventory&quot;.

![]({{ site.baseurl }}/assets/images/rule_14.png)
