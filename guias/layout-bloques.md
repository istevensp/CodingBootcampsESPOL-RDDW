---
remote_theme: chrisrhymes/bulma-clean-theme
---
## Layout, bloques y herencia de plantillas

[Regresar](/CodingBootcampsESPOL-RDDW/)

+ Continuando con la parte de layout. Ahora se creará el archivo layout.html en la carpeta de templates.

```
<body>
        <h1> Sitio web con Django </h1>
    <hr/>
    <ul>
        <li>
            <a href="/inicio"> Inicio </a>
        </li>
        <li>
            <a href="/hola-mundo"> Hola Mundo </a>
        </li>
        <li>
            <a href="/pagina-pruebas"> Página de prueba </a>
        </li>
        <li>
            <a href="/contacto"> Contacto </a>
        </li>
    </ul>
    </hr>
    <div id="content">
        {% block content %}

            <!--Codigo que viene de templates-->
        {% endblock %}

    </div>
    <footer>
        Master en Python &copy;
    </footer>
</body>
```