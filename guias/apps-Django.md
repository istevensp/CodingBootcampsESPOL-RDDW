## Creación de apps de Django

[Regresar](/CodingBootcampsESPOL-RDDW/)

Una app es un paquete que va formando nuestro proyecto web para ir trabajando en distintas secciones de la aplicación. Y cada app tiene su funcionalidad dentro de la aplicación. En la clase anterior creamos nuestro [primer proyecto en Django](./primer-proyecto-Django.md) en donde dentro de la carpeta AprendiendoDjango se encuentra una subcarpeta con el mismo nombre, ahi encontrarás el archivo settings.py que contiene la información de las apps instaladas. 

+ Abrimos la terminal y nos ubicamos en la carpeta AprendiendoDjango que fue generada en el [primer proyecto en Django](./primer-proyecto-Django.md). 

+ Generaremos la app con el nombre de "miapp" ejecutando el siguiente comando en la consola. 

```
python manage.py startapp miapp
```
Con la ejecución del comando anterior se generó la subcarpeta miapp que contiene los distintos archivos para empezar a configurar la app de Django. 