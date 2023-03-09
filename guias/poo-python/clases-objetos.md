## Clases y objetos

+ Crea una carpeta RDDD donde se encontrarán los ejercicios para cada tema propuesto. Dentro de esa carpeta crearás un subcarpeta con el nombre POO-clases.

+ En la carpeta POO-clases, crea un archivo main.py. 

Tengamos en consideración que una clase es un molde para crear más objetos de ese tipo con características similares.

+ En el archivo main.py, definiremos una clase Coche con la siguiente línea de código

  ```Python
  class Coche:
  ```

+ A la clase Coche se le definirán los atributos de color, marca, modelo, velocidad, caballaje y plazas.

```Python
class Coche: 

    # Atributos o propiedades
    color = "Rojo"
    marca = "Ferrari"
    modelo="Aventador"
    velocidad = 300
    caballaje = 500
    plazas = 2
```

 Ahora a nuestra clase Coche le definiremos métodos que son accciones del objeto. Es importante conocer que con la palabra reserva **self** se puede acceder a los atributos del objeto. La palabra reservada **self** se la pasa como parámetro y así dentro del método podremos acceder a todos los atributos. 

 + Crear un método con el nombre acelerar que aumente en 1 la velocidad del coche.

```Python
    def acelerar(self):
        self.velocidad += 1

```

+ Otro método que se creará es el de frenar que disminuye en 1 a la velocidad.

```Python
   def frenar(self):
        self.velocidad -= 1

```

+ También será necesario tener un obtenga para obtner la velocidad.

```Python
def getVelocidad(self):
        return self.velocidad

```
+ Ya definiendo la clase, se empezará con la creación de objetos. 

```Python
coche = Coche()
```

+ A partir del objeto cohe que fue creado, se accederá al atributo velocidad e imprimir su valor. 

```Python
print("Velocidad actual: ", coche.velocidad)
```

+ Para la clase coche, utilizaremos el método acelerar y frenar, posterior verificaremos el nuevo valor de la velocidad.

```Python
coche.acelerar()
coche.acelerar()
coche.acelerar()
coche.frenar()

print("Velocidad nueva: ", coche.velocidad)
```
El código final para el tema de clases y objetos tendría la siguiente estructura.

```Python
# Programación orientada a objetos

#Definir una clase

class Coche: 

    # Atributos o propiedades
    color = "Rojo"
    marca = "Ferrari"
    modelo="Aventador"
    velocidad = 300
    caballaje = 500
    plazas = 2

    # Métodos, son acciones que hace el objeto Coche

    def acelerar(self):
        self.velocidad += 1

    def frenar(self):
        self.velocidad -= 1

    def getVelocidad(self):
        return self.velocidad
    
#fin definición clase

#Crear objetos / Instanciar la clase

coche = Coche()

print(coche.marca, coche.color)

print("Velocidad actual: ", coche.velocidad)

coche.acelerar()
coche.acelerar()
coche.acelerar()
coche.frenar()

print("Velocidad nueva: ", coche.velocidad)
```
