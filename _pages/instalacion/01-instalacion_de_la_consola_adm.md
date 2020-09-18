---
title: Instalación de la consola ADM
chapter: "instalacion"
---

El instalador `Aranda.ADM.Web.Installer` de la consola web de ADM, instala los sitios de la consola y el Repserver; adicionalmente crea los servicios de los Crunchers, License, Scheduler, Mailer y Worker que se usan en la aplicación. A continuación, el paso a paso de la instalación.

Haga clic sobre el instalador, se visualizará la siguiente advertencia:

![]({{ site.baseurl }}/assets/images/cons_1.png)

En la siguiente pantalla se visualizará un mensaje informando que se va a instalar Aranda Device Management, haga clic en **Siguiente** para continuar.

![]({{ site.baseurl }}/assets/images/consv_2.png)

Ingrese el nombre de usuario y la organización donde se está instalando la aplicación.

![]({{ site.baseurl }}/assets/images/cons_3.png)

Visualizará el siguiente formulario:

![]({{ site.baseurl }}/assets/images/cons_4.1.png)

Ingrese los datos de autenticación de base de datos.
Existen dos formas de autenticación: Windows y SQL, ingrese el nombre de la base de datos y haga clic en **Siguiente**.

![]({{ site.baseurl }}/assets/images/cons_4.png)

Existen dos tipos de instalación: completa y personalizada. Seleccione instalación completa y haga clic en **Siguiente**.

![]({{ site.baseurl }}/assets/images/consv_3.png)

Ahora haga clic en **Instalar**.

![]({{ site.baseurl }}/assets/images/consv_4.png)
![]({{ site.baseurl }}/assets/images/cons.6.png)
![]({{ site.baseurl }}/assets/images/consv.7.png)
![]({{ site.baseurl }}/assets/images/consv_5.png)

Una vez culminado el proceso de instalación, haga clic en **Finalizar**.

### Requisitos de configuración del IIS en autenticación por Windows

En caso de que tenga habilitada la autenticación por Windows así:

![]({{ site.baseurl }}/assets/images/requisiti_01.png)

Deberá configurar el IIS para que no habilite la autenticación por formularios.

![]({{ site.baseurl }}/assets/images/IIS_1.png)

De esta manera se logra un buen funcionamiento de la aplicación.
