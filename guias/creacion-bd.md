## Creación de base de datos

[Regresar](/CodingBootcampsESPOL-RDDW/)

Durante el curso hemos trabajado con el directorio de RDDD-apps, así que en esta sección crearemos una nueva carpeta con el nombre de base-datos. En la carpeta de base de datos se creará un archivo main.py. 

+ En el archivo main.py importamos el conector de mysql.

```Python
import mysql.connector
```

+ Ahora realizaremos la conexión a la base de datos.

```Python
database = mysql.connector.connect(
    host="localhost",
    user="root",
    passwd=""
)
```

+ Para verificar la conexión realizaremos un print. El resultado nos debe mostrar que es un objeto de tipo conector. Recuerde que para visualizar el resultado, en la terminal debe ubicar en la carpeta de base de datos e ejcutar con el código de python `main.py`.

```Python
print(database)
```
+ Es momento de crear nuestra base de datos, master_python será el nombre de la base de datos a crear.

```Python
cursor = database.cursor()
cursor.execute("CREATE DATABASE IF NOT EXISTS master_python")
```

+ La verificación de que se creó la base de datos es con la instrucción de `main.py` que se añadirá en el archivo main.py.

```Python
cursor.execute("SHOW DATABASES")
for bd in cursor:
    print(bd)
```
+ Ejecutamos en la terminal el archivo main.py con `python main.py`. Ahí verificamos que se encuentre la base de datos master_python.

+ Actualizamos el código de database, en donde se debe añadir el campo de database con nombre de la base de datos.

```Python
database = mysql.connector.connect(
    host="localhost",
    user="root",
    passwd="recalde26",
    database="master_python"
)
```