## Servicio de licenciamiento {#servicio-de-licenciamiento}

ADM utiliza el servicio común de licenciamiento de Aranda para autorizar el ingreso a usuarios a la consola y controlar las licencias compradas, entre otras operaciones.
Este es un servicio de Windows que normalmente es creado de manera automática por el instalador del producto.
Una vez el usuario cargue desde la consola sus licencias compradas, el servicio común de licenciamiento debe permanecer en la misma máquina, de otra manera las licencias cargadas se perderán.
Si su servidor de aplicaciones se encuentra ubicado en una máquina virtual recomendamos altamente instalar el servicio común de licenciamiento en una máquina física, ya que al reiniciar máquinas virtuales existe una alta probabilidad de que la marca de hardware cambie y el servicio asuma incorrectamente que fue trasladado.

Consulte con el proveedor para más detalles sobre el despliegue del servidor.