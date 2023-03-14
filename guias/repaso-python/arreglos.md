## Arreglos

[Regresar](/CodingBootcampsESPOL-RDDW/)

Arreglos N-dimensionales
===========

* * *

Agrupación de elementos del mismo tipo de dato  (homogéneos) y con un tamaño definido.

+ **Dimensión 1:** Arreglos
[2 3 4]

+ **Dimensión 2:** Matriz
[[2 3 4]
[4 3 4]]

Numpy
===========

* * *

Librería de Python que permite realizar  operaciones con arreglos n-dimensionales  (arreglos y matrices).

```python
import numpy as np
```


<p align="center">
<img src="https://miro.medium.com/v2/1*cyXCE-JcBelTyrK-58w6_Q.png" width="40%" alt="Banner"/>
</p>

Creación de arreglos
===========

* * *
Creando un arreglo a partir de una lista.

<p align="center">
<img src="../imagenes/arreglo.png" width="40%" alt="Banner"/>
</p>

Cuando se crea un arreglo se puede especificar el tipo de dato de los  elementos que tendrá el arreglo.

<p align="center">
<img src="../imagenes/arreglo2.png" width="40%" alt="Banner"/>
</p>

Errores de creación de arreglos
===========

* * *

a = np.array(1,2,3,4)     ❌

b = np.array ([1,2,3,4])  ✅ 

Propiedades de arreglos n-dimensionales
===========

* * *

<p align="center">
<img src="../imagenes/arreglos-n.png" width="40%" alt="Banner"/>
</p>
<p align="center">
<img src="../imagenes/propiedades.png" width="40%" alt="Banner"/>
</p>

Propiedades de las matrices
===========

* * *

<p align="center">
<img src="../imagenes/matrices.png" width="40%" alt="Banner"/>
</p>

Inicialización de arreglos n-dimensionales
===========

* * *

<p align="center">
<img src="../imagenes/inicializacion.png" width="40%" alt="Banner"/>
</p>

<p align="center">
<img src="../imagenes/ini.png" width="40%" alt="Banner"/>
</p>

Inicialización de matrices
===========

* * *

<p align="center">
<img src="../imagenes/matri.png" width="40%" alt="Banner"/>
</p>

<p align="center">
<img src="../imagenes/matri2.png" width="40%" alt="Banner"/>
</p>

Modificar arreglos n-dimensionales
===========

* * *

+ **Fill:** Llena las posiciones de un arreglo previamente creado con valor específico.

<p align="center">
<img src="../imagenes/modificacion.png" width="40%" alt="Banner"/>
</p>

+ **Concatenate:** Permite concatenar 2 o más arreglos n-dimensionales.

<p align="center">
<img src="../imagenes/concatenate.png" width="40%" alt="Banner"/>
</p>

Operaciones con escalares
===========

* * *

Se puede realizar operaciones aritméticas entre los arreglos n-  dimensionales y escalares. El resultado de esta operación afecta a los  elementos del arreglo n-dimensional.

<p align="center">
<img src="../imagenes/escalares.png" width="40%" alt="Banner"/>
</p>

Operaciones en arreglos n-dimensionales
===========

* * *

<p align="center">
<img src="../imagenes/dimensionales.png" width="40%" alt="Banner"/>
</p>

<p align="center">
<img src="../imagenes/dimensionales2.png" width="40%" alt="Banner"/>
</p>

Operaciones en matrices
===========

* * *

<p align="center">
<img src="../imagenes/opmatrices.png" width="40%" alt="Banner"/>
</p>

Operaciones adicionales
===========

* * *

<p align="center">
<img src="../imagenes/adicionales.png" width="40%" alt="Banner"/>
</p>

Asignaciones en arreglos
===========

* * *

<p align="center">
<img src="../imagenes/asignacion4.png" width="40%" alt="Banner"/>
</p>

Slicing en arreglos
===========

* * *

<p align="center">
<img src="../imagenes/slicing.png" width="40%" alt="Banner"/>
</p>

Slicing en matrices
===========

* * *

<p align="center">
<img src="../imagenes/slicing2.png" width="40%" alt="Banner"/>
</p>

Funciones en arreglos n-dimensionales
===========

* * *

<p align="center">
<img src="../imagenes/funciones.png" width="40%" alt="Banner"/>
</p>

Operaciones básicas
===========

* * *
<p align="center">
<img src="../imagenes/opbasicas.png" width="40%" alt="Banner"/>
</p>

Operaciones estadísticas
===========

* * *
<p align="center">
<img src="../imagenes/opest.png" width="40%" alt="Banner"/>
</p>

<p align="center">
<img src="../imagenes/opest2.png" width="40%" alt="Banner"/>
</p>

Función arange: arreglos
===========

* * *

<p align="center">
<img src="../imagenes/arange.png" width="40%" alt="Banner"/>
</p>

Transformar un arreglo en matriz:  reshape
===========

* * *

La	función	reshape	recibe	la	forma	del	nuevo	arreglo	n	dimensional.	La  forma debe corresponder a la cantidad de elementos que tiene el arreglo.

<p align="center">
<img src="../imagenes/reshape.png" width="40%" alt="Banner"/>
</p>

Función reshape: matrices
===========

* * *

<p align="center">
<img src="../imagenes/reshape2.png" width="40%" alt="Banner"/>
</p>

Transformar una matriz en un  arreglo: ravel
===========

* * *
La función ravel transforma cualquier arreglo n-dimensional en un arreglo  de una dimensión.

<p align="center">
<img src="../imagenes/ravel.png" width="40%" alt="Banner"/>
</p>

Función where
===========

* * *
Retorna un nuevo arreglo a partir de 2 arreglos (x, y), con elementos que  dependen de una condición booelana. La condición booleana es usada como  filtro para elegir entre elementos de los 2 arreglos.


<p align="center">
<img src="../imagenes/where.png" width="40%" alt="Banner"/>
</p>

Función en matrices (copy)
===========

* * *
<p align="center">
<img src="../imagenes/copy.png" width="40%" alt="Banner"/>
</p>

Indexación booleana
===========

* * *
<p align="center">
<img src="../imagenes/indexacion.png" width="40%" alt="Banner"/>
</p>

<p align="center">
<img src="../imagenes/indexacion2.png" width="40%" alt="Banner"/>
</p>