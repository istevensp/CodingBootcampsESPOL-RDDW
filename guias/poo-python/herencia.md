## Herencia

[Regresar](/CodingBootcampsESPOL-RDDW/)

Para la ejemplicación de la herencia, dentro del directorio de RDDD-apps crearemos la carpeta POO-herencia. A su vez tendrá los archivos main.py y clases.py. 

Recordemos que a la herencia la podemos definir como la posibilidad de compartir atributos y métodos entre clases. Y que diferentes clases herede de otras.

+ En el archivo clases.py crearemos la clase Persona y definiremos propiedades como nombre, apellido, altura y edad. Para esos atributos implementamos los getters y setters. Luego definimos una serie de métodos como: hablar, caminar y dormir que son comportamientos génericos de las personas. 

```Python
class Persona:

    #getters y setters
    def getNombre(self):
        return self.nombre 
    
    def getApellido(self):
        return self.apellidos
    
    def getAltura(self):
        return self.altura
    
    def getEdad(self):
        return self.edad 
    
    def setNombre(self, nombre):
        self.nombre = nombre

    def setApellidos(self, apellidos):
        self.apellidos = apellidos
    
    def setAltura(self, altura):
        self.altura = altura

    def setEdad(self, edad):
        self.edad = edad
    
    #Métodos

    def hablar(self):
        return "Estoy hablando"
    def caminar(self):
        return "Estoy caminando"
    def dormir(self):
        return "Estoy durmiendo"
```

+ Ahora definiremos la clase Informatico que heredera de la clase padre Persona. Para ello cuando se define la clase Informatico dentro del parántesis colococar el nombre de la clase de la cuál se quiere herederar. Definimos un método constructor que tendrá los atributos lenguaje y experiencia que son propios de la clase Informatico. Además se implementaron los métodos aprender, programar y repararPC.

```Python
class Informatico(Persona):
    def ___init__(self):
        self.lenguajes = "HTML, CSS, JavaScript, PHP"
        self.experiencia = 5

    def getLenguajes(self):
        return self.lenguajes
    
    def aprender(self, lenguajes):
        self.lenguajes = lenguajes
        return self.lenguajes
    
    def programar(self):
        return "Estoy programando"
    
    def repararPC(self):
        return "He reparado tu ordenador"
```
Debemos tener en cuenta que la clase Informatico tendra todos los métodos y atributos de la clase padre. A continuación realizaremos un serie de ejemplo sobre herencia.

+ En el archivo main.py se debe importar el archivo clases.py. Luego, se creará un objeto de tipo Persona seteandole sus atributos e imprimiéndolos.

```Python
import clases 

persona = clases.Persona()
persona.setNombre("Victor")
persona.setApellidos("Robles")
persona.setAltura("170cm")
persona.setEdad("800 años")

print(f"La persona es: {persona.getNombre()} {persona.getApellido()}")
print(persona.hablar())
```
+ Ahora ejemplificaremos la clase Informatico. Creamos el objeto de tipo informatico y seteandole sus atributos. 

```Python
informatico = clases.Informatico()
informatico.setNombre("Carlos")
informatico.setApellidos("Martinez")
print(f"El informatico es: {informatico.getNombre()} {informatico.getApellido()}")
print(informatico.hablar())
print(informatico.caminar())
```
