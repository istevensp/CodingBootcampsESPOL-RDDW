## Colecciones

[Regresar](/CodingBootcampsESPOL-RDDW/)

Diccionarios
===========

* * *

Un diccionario es una versión general de una lista. Aquí hay una lista que contiene el número de días en los meses del año.

```python
días = [31, 28, 31, 45, 78]
```
Si queremos el número de diás de enero, utilice días[0]. Diciembre es días[11] o días[-1].
Aquí hay un diccionario:

```python
días = {"Enero":31, "Febrero":28, "Marzo":31, "Abril":30}
```

<p align="center">
<img src="https://blog.facialix.com/wp-content/uploads/2019/08/diccionarios.png" width="40%" alt="Banner"/>
</p>

Declaración de diccionarios
===========

* * *

```python
dic = {"A":100, "B":200}
```

+ Para declarar diccionarios lo encerramos entre llaves, {}. 
+ Cada entrada consiste en un par separado por dos puntos.
+ La primera parte del par se llama clave y la segunda es el valor.
+ La clave actúa como índice. Así que en el primer par, "A":100, la clave es "A", el valor es 100.

- Para cambiar dic["A"] a 400, realice lo siguiente:
    dic["A"]=400
- Para agregar una nueva entrada al diccionario, simplemente se hace una asignación.
    dic["C"]=500
- Para eliminar una entrada de un diccionario, use el operador **del**.
    del dic["A"]

Ejemplos de diccionarios
===========

* * *

Puede usar un dicccionario como un diccionario real de definiciones:
```python
dic = {"perro":"tiene coloa y hace guau!", "gato":"hace maullido", "ratón":"perseguido por gatos"}
```

```python
word = input('Ingrese una palabra: ')
print('La definición es:', dic[word])
#OUTPUT
Ingrese una palabra: gato
La definición es: hace maullido
```
El siguiente diccionario es útil en un programa que trabaja con números romanos. 

```python
romanos = {'I':1, 'V':5, 'X':10, 'L':50, 'C':100, 'D':500, 'M':1000}
```

Trabajar con diccionarios
===========

* * *

+ Copiar dicccionarios al igual que las listas es un poco complicado. Sin embargo, utilice su método de copia. 

```python
d2 = d.copy()
```
+ El operador **in** se usa para saber si algo es una clave en el diccionario. Por ejemplo se tiene el siguiente diccionario. 

```python
d = {'A':100, 'B':200}
```
Hacer referencia a una clave que no está en el diccionario producirá error. Por ejemplo `d[C]` producirá error. Para evitar este error, se puede usar el operador **in** para verificar primero si una clave está en el diccionario antes de intentar usar la clave. 

```python
letter = input('Enter a letter: ')
if letter in d:
    print('The value is', d[letter])
else:
    print('Not in dictionary')
```
+ El operador **not in** se usa para ver si una clave no está en el diccionario. 

Tuplas
===========

* * *
 Una tupla es esencialmente una lista inmutable. A continuación, se muestra una lista con tres elementos y una tupla con tres elementos.

 ```python
L = [1,2,3]
t = (1,2,3)
```
<p align="center">
<img src="https://aprendepython.es/_images/tuple-unpacking.jpg" width="40%" alt="Banner"/>
</p>

Las tuplas se encierran entre paréntesis, aunque los paréntesis en realidad son opcionales. La indexación funcionan igual que con las listas. Una de las razones por las que existen listas y tuplas es que, es posible que desee un tipo de lista inmutable. 

Conjuntos
===========

* * *

Python tiene un tipo de dato llamado conjunto. Los conjuntos funcionan como conjuntos matemáticos. Se parecen mucho a las listas sin repeticiones. Los conjuntos se denotan con llaves. 

 ```python
S = {1,2,3,4,5}
```
Recuerde que las llaves también se usan para indicar diccionarios y {} es el diccionario vacío. Para obtener el conjunto vacío, use la función **set** sin argumentos.
 ```python
S = set()
```
La función **set** también se puede usar para convertir cosas en conjuntos.

 ```python
set([1,4,4,4,5,1,2,1,3])
set('this is a test')
```

<p align="center">
<img src="https://www.lifeder.com/wp-content/uploads/2019/12/Conjunto-01.jpg" width="40%" alt="Banner"/>
</p>