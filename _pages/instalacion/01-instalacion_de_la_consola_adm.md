---
title: Instalación de la consola ADM
chapter: "instalacion"
---

El instalador `Aranda.ADM.Web.Installer` de la consola web de ADM, instala los sitios de la consola y el Repserver; adicionalmente crea los servicios de los Crunchers, License, Scheduler, Mailer y Worker que se usan en la aplicación. A continuación, el paso a paso de la instalación.

Haga clic sobre el instalador, se visualizará la siguiente advertencia:

En la siguiente pantalla se visualizará un mensaje informando que se va a instalar Aranda Device Management, haga clic en **Siguiente** para continuar.

Ingrese el nombre de usuario y la organización donde se está instalando la aplicación.

Visualizará el siguiente formulario:

Ingrese los datos de autenticación de base de datos.
Existen dos formas de autenticación: Windows y SQL, ingrese el nombre de la base de datos y haga clic en **Siguiente**.

Existen dos tipos de instalación: completa y personalizada. Seleccione instalación completa y haga clic en **Siguiente**.

Ahora haga clic en **Instalar**.

Una vez culminado el proceso de instalación, haga clic en **Finalizar**.

## Requisitos de configuración del IIS en autenticación por Windows {#requisitos-de-configuraci-n-del-iis-en-autenticaci-n-por-windows}

En caso de que tenga habilitada la autenticación por Windows así:

Deberá configurar el IIS para que no habilite la autenticación por formularios.

De esta manera se logra un buen funcionamiento de la aplicación.
