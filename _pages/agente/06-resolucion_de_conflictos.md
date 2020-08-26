---
title: Resolución de conﬂictos
chapter: "agente"
---

Desde la versión 9.5 la consola de administración de ADM permite visualizar y gestionar fácilmente los potenciales problemas de identificación que ocurren a los dispositivos. Estos problemas se conocen como conflictos y son mostrados en la hoja de vida de los dispositivos para que el usuario tome una decisión sobre cada uno de ellos. De esta manera se evitan más fácilmente inconsistencias como la suplantación de máquinas y la duplicidad de registros. La suplantación ocurre cuando muchos dispositivos se ven como uno solo en la consola, como efecto de clonación de equipos que ya tienen instalado el agente, principalmente. La duplicidad ocurre cuando una máquina tiene mas de un registro asociado en la consola, normalmente es debido al ingreso de máquinas que fueron formateadas después de tener agente instalado.

Todo agente instalado en un dispositivo realiza periódicamente una operación de registro con su servidor, en donde se envían tres valores: una marca de hardware, la identificación asignada por el servidor y un token dinámico. Si alguno de estos valores no coincide con el que el servidor espera se bloquean permanentemente las solicitudes de este equipo y se muestra un conflicto en la hoja de vida respectiva en consola. El usuario debe entonces resolver el conflicto eligiendo una acción a tomar cuando la solicitud de registro sospechosa vuelva a presentarse. Cuando se presente la siguiente solicitud el conflicto quedará resuelto.

Todas las máquinas que presenten conflictos serán marcadas y podrán ser filtradas en el listado para que el usuario pueda gestionarlas fácilmente.

![agen_9]({{ site.baseurl }}/assets/images/agen_9.png)

Al entrar a la hoja de vida el usuario verá una lista con todos los conflictos detectados para una máquina, para cada conflicto se indica el tipo y se muestra un selector para la acción a tomar. Los conflictos pueden ser de tres tipos: Hardware duplicado, Hardware inconsistente e identificador duplicado. La pestaña de ayuda en este pantalla explica cada uno de ellos y explica cómo deben resolverse.

![agen_10]({{ site.baseurl }}/assets/images/agen_10.png)

Las aciones a tomar son Asociar dispositivo, Crear dispositivo o aplazar la decisión dejándo la acción Pendiente. El usuario podría también Borrar el conflicto si considera que ya no volverá a ocurrir.

![agen_11]({{ site.baseurl }}/assets/images/agen_11.png)

Es posible que el usuario sepa de antemano qué un tipo específico de conflicto se presentará muy frecuentemente para una máquina. Por ejemplo, si una máquina virtual fue clonada muchas veces después de tener el agente instalado y se pretende ingresar todos los clones al sistema (generando conflictos de identificador duplicado), o si una máquina física es formateada y regingresada cada semana para ser usada en campañas diferentes (generando conflictos de hardware duplicado). En estos casos los conflictos son predecibles y el usuario puede configurar una acción automática en la hoja de vida.

![agen_12]({{ site.baseurl }}/assets/images/agen_12.png)
