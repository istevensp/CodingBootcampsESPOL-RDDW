## Tipado de objetos

[Regresar](/CodingBootcampsESPOL-RDDW/)

Para hacer la detección del tipado de objeto utilizaramos los archivos creados en la clase de[constructores](./constructor.md). En este caso para verificar el tipado de objeto se utiliza la palabra reservada **type**.

+ En el archivo main.py hacer la validación del tipado con el siguiente código.

```Python
#Detectar tipado

if type(carro2) == Coche:
    print("Es un objeto correcto !!")
else:
    print("No es un objeto!!")
```
+ En la terminal ejecutamos el comando `python main.py` y nos dará como resultado **Es un objeto correcto !!** 

+ Para verificar que no es un objeto agregamos la siguiente linea de codigo:

```Python
carro2 = "Aleatorio"
```
Con la modificación anterior, volvemos a ejecutar el archivo main.py y ahora nos dará como resultado **No es un objeto!!**.