## Diseño de la web empresarial

[Regresar](/CodingBootcampsESPOL-RDDW/)

Para esta sección de proyecto crearemos una web empresarial donde se encontrará información como el catálogo de servicios, información de la empresa, entre otras funcionalidades que se irán desarrollando.
* En la sección de [recursos](./webempresa_Frontend.zip) se encontrará una plantilla de frontend de una cafetería que se estará utilizando en el proyecto.

En el backend siempre se debe verificar y diferenciar cuáles son las páginas estáticas y dinámicas. Las páginas estáticas hacen referencia a que la información se mantendrá a lo largo del tiempo, en cambio, las dinámicas son aquellas que su contenido si sera modificado mediante el panel de amdministración. 
En este proyecto de la cafetería las páginas estáticas son:
* Portada
* Historia
* Visítanos

Las páginas dinámicas serán:
* Servicio
* Blog

Dado el análisis anterior nuestro proyecto tendrá 6 apps para la parte del backend.  
* La app core gestionará las páginas estáticas: portada, historia y visítanos.
* La app services para gestionar los servicios.
* La app blog para gestionar las entradas y categorías del blog. 
* La app social para manejar las redes sociales. 
* La app pages para manejar las páginas secundarias. 
* La app contact para manejar la parte del contacto en el formulario.