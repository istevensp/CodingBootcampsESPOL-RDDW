## Creación de vistas y Rutas

[Regresar](/CodingBootcampsESPOL-RDDW/)

Creación de vistas
===========

* * *

En el la sección anterior de [apps de django](./apps-Django.md) creamos la app y continuaremos con ese proyecto. Nos ubicamos en la carpeta AprendiendoDjango y en la subcarpeta miapp se encuentra el archivo views.py en dicho archivo estaremos trabajando. 

+ En el archivo views.py, crearemos un ejemplo para ilustrar el tema de las vistas. Copie el siguiente código en el archivo.

```python
from django.shortcuts import render, HttpResponse

# Create your views here.

def holaMundo(request):
    return HttpResponse("Hola mundo con Django!!")
```

+ Es momento de abrir la terminal ubicandose en la carpeta de AprendiendoDjango, y ejeuctar el comando:

```
python manage.py runserver
```

+ Copia la URL que se obtuvó al ejecutar el comando anterior, copia dicho enlace y debes abrirlo en tu navegador. 

+ Es momento de configurar una URL y así visualizar los cambios realizaos en la vista. 

+ Dentro del proyecto general de AprendiendoDjango se encuentra una subcarpeta con el mismo nombre y ahí se encontrará el archivo urls.py  y agregamos la ruta. 

```python
from django.contrib import admin
from django.urls import path

from miapp import views 
urlpatterns = [
    path('admin/', admin.site.urls),
    path('hola-mundo/', views.hola_mundo, name="hola_mundo")
]
```

+ En el navegador web coloca la url que salia de la ejecución además de agregarle el hola-mundo/. Y de ese forma se consigue la ejecuón del Hola Mundo. 

Y asi se visualizará el "Hola mundo con Django!!". 