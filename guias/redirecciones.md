## Redirecciones

[Regresar](/CodingBootcampsESPOL-RDDW/)

+ Continuamos trabajando el el proyecto de AprendiendoDjango, en el archivo views.py añadir las siguientes líneas de código en la variable layout y así actualizar el menú de navegación. 

```
<li>
        <a href="/contacto"> Contacto </a>
</li>
```

+ Para la página de prueba agregamos un parámetro opcional. Agregamos lo siguiente en el archivo urls.py. 

```python
path('pagina-pruebas/<int:redirigir>', views.pagina, name="pagina")
```
+ Ese parámetro debe ser agregado en la función pagina del archivo views.py.

```python
def pagina(request, redirigir=0):
    if redirigir ==1:
        return redirect("/contacto/")
    return HttpResponse(layout+
        """
        <h1> Página de mi web </h1>
        """
    )
```