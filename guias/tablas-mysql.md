## Tablas en mysql

[Regresar](/CodingBootcampsESPOL-RDDW/)

Ahora siguiendo con el tema de base de datos, continuaremos con la creación de tablas para la base de datos master_python que fue creada en la sección de [creación de base de datos](./creacion-bd.md).

+ Iniciaremos creando la tabla vehiculos con los campos de id, marca, modelo, precio. Las siguientes líneas de código deben ser agregadas en el archivo main.py donde se venia trabajando en la sección de [creación de base de datos](./creacion-bd.md).

```Python
cursor.execute(""""
CREATE TABLE IF NOT EXISTS vehiculos(
    id int(10) auto_increment not null,
    marca varchar(40) not null,
    modelo varchar(40) not null,
    precio float(10,2) not null,
    CONSTRAINT pk_vehiculo PRIMARY KEY(id)
)
""")
```
+ Abra la terminal en la carpeta base-datos y de ahí ejecute el comando `python main.py`

+ Mediante codigo verificaremos que efectivamente se creó la tabla.

```Python
cursor.execute("SHOW TABLES")
for table in cursor:
    print(table)
```

Insertar registros
===========

* * *

+ Con las siguientes isntrucciones ingresaremos datos a nuestra tabla vehiculos. 

```Python
cursor.execute("INSERT INTO vehiculos VALUES(null, 'Opel', 'Astra', 18500)")
#Guarda los cambios
database.commit()
```

+ Existe otra alternativa de insertar registros de forma masiva. 

```Python
#lista con los distintos coches
coches = [
    ('Seat','Ibiza', 5000),
    ('Renault','Clio', 15000),
    ('Citroen','Saxo', 2000),
    ('Mercedes','Clase C', 35000)
]
cursor.executemany("INSERT INTO vehiculos  VALUES (null, %s, %s, %s)", coches)
database.commit()
```

SELECT
===========

* * *

La instrucción SELECT de MySQL se utiliza para recuperar registros de una o más tablas en MySQL pudiendo seleccionar cuales campos queremos incluir y excluir. Su sintaxis es la siguiente:

```sql
SELECT campos
FROM tablas
[WHERE condiciones];
```
+ Para realizar las consultas de todos los vehículos que se encuentran en la tabla, utilizamos el siguiente código.

```Python
cursor.execute("SELECT * FROM vehiculos")
result = cursor.fetchall()
print("----TODOS MIS COCHES----")
for coche in result:
    print(coche)
```
+ Si queremos obtener solo la marca del coche hacemos la modificación en el print. 

```Python
cursor.execute("SELECT * FROM vehiculos")
result = cursor.fetchall()
print("----TODOS MIS COCHES----")
for coche in result:
    print(coche[1])
```
+ Si deseamos obtener la marca y el precio utiliza los siguiente:

```Python
cursor.execute("SELECT * FROM vehiculos")
result = cursor.fetchall()
print("----TODOS MIS COCHES----")
for coche in result:
    print(coche[1], coche[3])
```
+ Si deseamos obtener los vehiculos que tengan un precio menor o igual a 5000 utilizamos la cláusula **WHERE**.

```Python
cursor.execute("SELECT * FROM vehiculos WHERE precio <= 5000")
result = cursor.fetchall()
print("----TODOS MIS COCHES----")
for coche in result:
    print(coche[1], coche[3])
```

+ Ahora haremos una consulta que nos permita obtener los vehiculos que tengan un precio menor o igual a 5000 y además que sean de la marca SEAT.

```Python
cursor.execute("SELECT * FROM vehiculos WHERE precio <= 5000 AND marca = 'Seat' ")
result = cursor.fetchall()
print("----TODOS MIS COCHES----")
for coche in result:
    print(coche[1], coche[3])
```
+ Ahora una consulta que nos devuelva la primera fila de nuestra tabla de vehículos. 

```Python
cursor.execute("SELECT * FROM vehiculos")
coche = cursor.fetchone()
print(coche)
```

Borrar registros
===========

* * *

Para eliminar registros utilizamos la cláusula **DELETE**.
+ Para evitar errores modificamos el cursor y le agregamos el parámetro buffered=TRUE.

```Python
cursor = database.cursor(buffered=True)
```
+ Ahora eliminaremos los vehículos que tengan la marca Renault.

```Python
cursor.execute("DELETE FROM vehiculos WHERE marca = 'Renault' ")
database.commit()
```

Actualizar registros
===========

* * *

Para modificar registros utilizamos la cláusula **UPDATE**.

+ Actualizaremos el modelo a Leon de los vehículos con marca Seat.

```Python
cursor.execute("UPDATE vehiculos SET modelo='Leon' WHERE marca = 'Seat'")
database.commit()
print(cursor.rowcount, "actualizados!")
```