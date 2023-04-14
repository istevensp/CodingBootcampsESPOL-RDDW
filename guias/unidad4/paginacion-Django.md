## Paginación en Django

[Regresar](/CodingBootcampsESPOL-RDDW/)

La Paginación en django es excelente, permite una flexibilidad importante para solucionar muchos problemas que se presentan al paginar resultados.

* En el archivo views.py(django\ProyectoDjango\blog\views.py) de la app blog para que en la sección de artículos nos muestre 1 artículo por página.

<p align="center">
<img src="../imagenes/paginar1.png" width="50%" alt="Banner"/>
</p>

* Actualiza el servidor y accede a las distintas páginas para los artículos. En este aso, configuramos para que se muestre 1 página por artículo.

<p align="center">
<img src="../imagenes/paginar4.png" width="50%" alt="Banner"/>
</p>

* Para la navegación de la paginación, agregamos un archivo pagination.html(django\ProyectoDjango\blog\templates\articles\pagination.html) con el siguiente código.

<p align="center">
<img src="../imagenes/paginar5.png" width="50%" alt="Banner"/>
</p>

* En el archivo de list.html(django\ProyectoDjango\blog\templates\articles\list.html) debes incluir el archivo de paginación.

<p align="center">
<img src="../imagenes/paginar6.png" width="50%" alt="Banner"/>
</p>

* Actualiza el navegador y visualiza los cambios.

<p align="center">
<img src="../imagenes/paginar3.png" width="50%" alt="Banner"/>
</p>