

# Database Fundamentals

Bienvenidos a la guía básica, para principiantes, sobre dockers realizada por Ramon Peinado Ruiz gracias al curso de accenture.



## CONCEPTOS BASICOS

### ¿Que es una base de datos ?

Una base de datos es un sistema organizado para recopilar, almacenar y gestionar datos de manera estructurada. Permite almacenar información de manera eficiente y proporciona un método para recuperar, actualizar y gestionar esos datos de manera rápida y segura. En esencia, una base de datos actúa como un almacén centralizado de información que puede ser accedida y manipulada por múltiples usuarios o sistemas.

<img align="center" src="/img/1ºimagenn.PNG"  />

**Ventajas de las bases de datos:**

**-Almacenamiento de Información:**

Las bases de datos posibilitan el almacenamiento eficiente de grandes cantidades de información, siendo cruciales para empresas con volúmenes significativos de datos. Además, facilitan el acceso, intercambio y eliminación ágil de datos.

**-Control de Seguridad:**

Los administradores de la Base de Datos pueden gestionar el acceso a la información, permitiendo o restringiendo la entrada a usuarios específicos.

**-Reducción de Redundancias:**

Evitan la duplicación de datos en varios archivos, lo que resulta en un menor volumen de datos y un acceso más rápido.

**-Accesibilidad Universal:**

Posibilitan la obtención de datos desde diversos contextos, aplicaciones y medios, volviéndolos útiles para un amplio número de usuarios.

**-Aumento de Productividad:**

Al consolidar todos los datos necesarios para las operaciones diarias en un único lugar, las bases de datos mejoran la eficiencia de las tareas y facilitan la toma de decisiones basada en la información disponible.

**-Consistencia de Datos:**

Previene discrepancias al evitar la existencia de valores distintos para un mismo dato.

 

### Tipos de bases de datos

#### **Según su variabilidad**:

**-Estáticas**

Las bases de datos con variabilidad estática permiten únicamente la lectura de información, sin la capacidad de realizar modificaciones en los datos ya existentes. Este tipo de bases de datos resulta útil para el almacenamiento de datos históricos, facilitando el estudio de su comportamiento a lo largo del tiempo y permitiendo realizar proyecciones futuras.

- Ejemplos: Censos, archivos históricos de bibliotecas,museos.

**-Dinámicas**

Por otro lado, las bases de datos con variabilidad dinámica no solo posibilitan la lectura de información, sino también la capacidad de actualizar, reorganizar, añadir y eliminar datos a lo largo del tiempo.

- Ejemplos: Base de datos utilizada en un supermercado o farmacia, redes sociales, sistemas de reservas en línea

#### **Según su contenido:**

**-Bibliográficas**

Las bases de datos bibliográficas son compilaciones de publicaciones científico-técnicas con el propósito de reunir toda la producción bibliográfica disponible sobre un área de conocimiento específica.

Ejemplos:

- **Repositorios Académicos**: Almacenan investigaciones, tesis y trabajos académicos, facilitando el acceso a la información científica.
- **Catálogos de Bibliotecas Digitales**: Recopilan recursos digitales, como libros electrónicos y documentos escaneados, para su consulta.

**-Directorios**

Estas bases de datos consisten en listados electrónicos de datos personales, como direcciones de correo electrónico o números de teléfono.

Ejemplos

- **Listados Empresariales**: Contienen información de contacto y detalles sobre empresas y profesionales en diversos sectores.
- **Agendas Telefónicas Digitales**: Recopilan números de teléfono y otra información de contacto para facilitar la comunicación.

**-De texto completo**

Bases de datos de texto completo recopilan artículos completos, permitiendo la búsqueda mediante términos específicos, palabras clave, fechas, entre otros.

Ejemplos:

- **Archivos de Periódicos Digitales**: Contienen ediciones completas de periódicos, permitiendo la búsqueda de noticias específicas.
- **Bases de Datos Jurídicas**: Almacenan textos legales completos, facilitando la investigación y referencia legal.

**-Especializadas**

Estas bases de datos contienen información altamente especializada o técnica, diseñadas para satisfacer las necesidades específicas de un público determinado.

Ejemplos:

- **Bases de Datos Médicas**: Contienen información detallada sobre enfermedades, tratamientos y estudios médicos, como PubMed.
- **Plataformas de Investigación Científica Especializada**: Ofrecen recursos específicos para campos como la biología molecular o la ingeniería genética.

### Modelos de bases de datos

Existen distintos modelos de bases de datos, y la manera en que la información se organiza dentro de una base de datos influye en las operaciones que se pueden llevar a cabo, como la lectura o modificación de datos. Surgen varios modelos en función de esta estructuración.

- Modelo Relacional: Tablas con filas y columnas, ampliamente utilizado, con lenguaje SQL para consultas y mantenimiento, modelo mas prevalente hoy en día. 
- Modelo Jerárquico: Estructura de árbol con relaciones Padre/Hijo, donde un padre puede tener varios hijos, pero cada hijo solo un padre.
- Modelo de Red: Registros interconectados formando una red mediante enlaces.
- Modelo Multidimensional: Representación en cubos de datos, con cada cara del cubo como una dimensión para los usuarios.
- Modelo de Datos Deductivos: Permite deducciones a partir de reglas y hechos almacenados.
- Modelo Orientado a Objetos: Datos y relaciones en una única estructura llamada objeto.
- Bases de Datos Transaccionales: Vinculadas a bases de datos relacionales, permiten el rápido envío y recepción de datos.
- Gestores de BBDD (DBMS): Sistemas que facilitan la creación, gestión y administración de bases de datos.
- Modelo Documental: Permite indexación para búsquedas poderosas y almacenamiento eficiente de grandes volúmenes de información.
- Modelo Orientado a Grafos: Representa información con nodos y aristas interconectadas.



## Bases de datos relacionales

Una Base de Datos Relacional es aquella que contiene y permite conectar distintas tablas de datos. Su objetivo es extraer información de interés o volver a montar los datos de maneras diferentes.

### Elementos

- **DATOS:**

  - Información objeto de estudio que se desea analizar.

- **COLUMNAS O ATRIBUTOS:**

  - Recogen los distintos valores que existen para un mismo atributo.
  - En una tabla, las columnas se identifican en vertical.

- **FILAS O REGISTROS:**

  - Conjunto de distintos atributos relacionados entre sí que contienen información sobre un mismo "sujeto".
  - Todas las filas de una misma tabla tienen la misma estructura y pueden estar desordenadas entre sí.
  - En una tabla, las filas se identifican en horizontal.

- **TABLA:**

  - Forma que toman los datos al ser registrada la información.
  - Compuesta por filas y columnas, similar a una plantilla de cálculo.
  - Una Base de Datos puede contener múltiples tablas según las necesidades.

  Ejemplo:

| ID Empleado | Nombre | Apellido  | Edad | Departamento  | Salario |
| ----------- | ------ | --------- | ---- | ------------- | ------- |
| 1           | Juan   | Pérez     | 30   | Ventas        | 50000   |
| 2           | María  | González  | 25   | Marketing     | 48000   |
| 3           | Carlos | Rodríguez | 35   | Finanzas      | 55000   |
| 4           | Laura  | Martínez  | 28   | Recursos Hum. | 52000   |

### **¿Cómo se conectan las tablas?**

Para establecer relaciones entre dos tablas, es necesario definir una clave foránea que se conecta con la clave primaria de otra tabla.

- **Clave Primaria (PK):**
  - Es una columna especial en la tabla que identifica de manera única cada valor.
  - Permite diferenciar un registro de otro.
- **Clave Foránea (FK):**
  - Es una columna que contiene el valor de la clave primaria de un registro en otra tabla.
  - Establece la "relación" entre dos registros.

<img align="center" src="/img/2ºimagenn.PNG"  />

### Gestores de bases de datos relacionales o *Data Base Managenent System (DBMS)*

Los sistemas de gestión de bases de datos, conocidos como DBMS, son fundamentales para organizar y recuperar información de manera eficiente. El modelo más comúnmente empleado por las empresas hasta ahora es el modelo relacional. Ahora, exploraremos algunos de los gestores de datos más prominentes:

- **Oracle:** Utilizado por aproximadamente el 60% de las empresas a nivel mundial, Oracle destaca por su vasta experiencia y una amplia gama de servicios. Coca-Cola es un ejemplo destacado de éxito al emplear este sistema.
- **MySQL:** Reconocido como el gestor de datos con licencia libre más popular, MySQL es capaz de soportar plataformas de gran envergadura como Facebook, Twitter, YouTube y LinkedIn, todas las cuales utilizan este gestor para el almacenamiento de datos.
- **PostgreSQL:** Gestionado por un grupo de desarrolladores altruistas, PostgreSQL está optimizado para ajustar su velocidad según el volumen de datos. Skype confía en este gestor para almacenar toda la actividad de chat y llamadas.
- **SQL Server:** Propiedad de Microsoft, SQL Server es capaz de poner a disposición grandes cantidades de datos simultáneamente para múltiples usuarios. Empresas destacadas como Telefónica han optado por este sistema.
- **SQLite:** Esta biblioteca en C permite transacciones de datos sin depender de un servidor o configuraciones complejas. Aunque no es adecuada para bases de datos muy grandes, Adobe lo utiliza como formato de archivo para la conocida aplicación Photoshop.
- **Apache Hive:** Construida sobre Hadoop, esta infraestructura de almacenamiento de datos proporciona agrupación, consulta y análisis de conjuntos de datos masivos. Empresas como Netflix y Amazon confían en Apache Hive para sus necesidades de almacenamiento.
- **DB2:** Propiedad de IBM, DB2 permite almacenar documentos completos para realizar operaciones y búsquedas. Destaca por su automatización, eliminando tareas rutinarias y proporcionando un almacenamiento de datos más liviano. Es la opción preferida para gestionar bases de datos generadas por las aplicaciones SAP.

## SQL

SQL es un lenguaje de programación diseñado para gestionar datos almacenados en BBDD relacionales.

### Funciones principales

- Creación de BBDD.
- Creación de nuevas tablas en una BBDD.
- Creación de procedimientos almacenados en una BBDD.
- Creación de vistas en una BBDD.
- Asignación de permisos en tablas, procedimientos y vistas.
- Consultas contra una BBDD.
- Recuperación de datos de una BBDD.
- Inserción de registros en una BBDD.
- Actualización de registros de una BBDD.
- Borrado de registros de una BBDD.

Permite mantener los datos precisos y seguros. Tambien ayuda a mantener la integridad de las BBDD:

- Fácil de aprender
- Lenguaje universal
- Lenguaje estable
- Lenguaje de uso trasversal
- Flexibilidad al acceder a datos

### Clasificacion de las SQL

**DDL -Data Definition Language:** Permite crear y modificar estructura de BBDD, sintaxis similar al lenguaje de programación.

**DCL - Data Control Language:** Permite crear roles, permisos e integridad referencial, asi como el control de acceso a la BBDD, sintaxis similar a lenguaje de programación.

**DML - Data Modification Language:**  Permite recuperar, almacenar, modificar,eliminar, insertar y actualizar datos de una BBDD.

**TCL - Transaction Control Language:** Permite administrar diferentes transacciones(Conjunto de ordenes ejecutadas de forma indivisible).

### Comandos Basicos:

#### Definicion - DDL :

- **CREATE:** Se utiliza para crear objetos en la base de datos, como tablas, índices, y vistas.

  ```sql
  CREATE TABLE Empleados (
      ID INT PRIMARY KEY,
      Nombre VARCHAR(50),
      Edad INT,
      Salario DECIMAL(10, 2)
  ); 
  ```

  Este comando crea una tabla llamada "Empleados" con columnas para ID, Nombre, Edad y Salario.

- **ALTER:** Permite modificar la estructura de los objetos existentes, como añadir o eliminar columnas en una tabla.

  ```sql
  ALTER TABLE Empleados
  ADD Departamento VARCHAR(30);
  ```

  Añade una nueva columna llamada "Departamento" a la tabla "Empleados".

- **DROP:** Elimina objetos de la base de datos, como tablas o índices.

  ```sql
  DROP TABLE Empleados; 
  ```

  Elimina la tabla completa de "Empleados" y todos sus datos.

- **TRUNCATE:** Elimina todos los registros de una tabla, pero mantiene su estructura.

  ```sql
  TRUNCATE TABLE Empleados;
  ```

  

  Elimina todos los registros de la tabla "Empleados", pero conserva su estructura.

#### Manipulación - DML

- **SELECT:**

  ```sql
  SELECT Nombre, Edad
  FROM Empleados
  WHERE Salario > 50000;
  ```

  Recupera los nombres y edades de los empleados cuyos salarios son mayores a 50,000.

- **INSERT:**

  ```sql
  INSERT INTO Empleados (ID, Nombre, Edad, Salario)
  VALUES (1, 'Juan Pérez', 30, 60000);
  ```

  Añade un nuevo empleado con ID 1, nombre "Juan Pérez", edad 30 y salario 60,000 a la tabla "Empleados".

- **UPDATE:**

  ```sql
  UPDATE Empleados
  SET Salario = Salario * 1.1
  WHERE Edad < 25;
  ```

  Incrementa el salario en un 10% para empleados menores de 25 años.

- **DELETE:**

  ```sql
  DELETE FROM Empleados
  WHERE Salario < 30000;
  ```

  Elimina los registros de empleados cuyo salario es menor a 30,000.

#### Clausulas 

- **FROM:**

   ```sql
   SELECT columna1, columna2
   FROM nombre_tabla
   WHERE nombre_columna = valor;
   ```

   La cláusula `FROM` especifica la tabla de la cual se van a seleccionar los registros.

- **ORDER BY:**

   ```sql
   SELECT columna1, columna2
   FROM nombre_tabla
   WHERE nombre_columna = valor
   ORDER BY columna1 ASC;
   ```

   La cláusula `ORDER BY` ordena los registros seleccionados según la columna especificada, ya sea de forma ascendente (`ASC`) o descendente (`DESC`).

- **LIMIT:**

   ```sql
   SELECT *
   FROM nombre_tabla
   LIMIT 10;
   ```

   La cláusula `LIMIT` limita el número de filas en el resultado de la consulta. En este caso, solo se seleccionarán las primeras 10 filas.

#### Operadores

- **Operadores de Comparación:**

  - `=`: Igual a
  - `<>` o `!=`: No igual a
  - `<`: Menor que
  - `>`: Mayor que
  - `<=`: Menor o igual a
  - `>=`: Mayor o igual a

  ```sql
  SELECT *
  FROM Empleados
  WHERE Salario > 50000;
  ```

  Selecciona todos los empleados cuyo salario es mayor a 50,000.

- **Operadores Lógicos:**

  - `AND`: Devuelve true si ambas condiciones son verdaderas.
  - `OR`: Devuelve true si al menos una de las condiciones es verdadera.
  - `NOT`: Invierte el resultado de una condición.

  ```sql
  SELECT *
  FROM Empleados
  WHERE Edad > 25 AND Departamento = 'Ventas';
  ```

  Selecciona empleados mayores de 25 años que trabajan en el departamento de Ventas.

#### Funciones de agregado:

- **COUNT:**

  Se utiliza para contar el número de filas en un conjunto de resultados.

  ```sql
  SELECT COUNT(ID)
  FROM Empleados;
  ```

  Devuelve el número de empleados en la tabla.

- **SUM:**

  Calcula la suma de los valores en una columna.

  ```sql
  SELECT SUM(Salario)
  FROM Empleados
  WHERE Departamento = 'Ventas';
  ```

  Devuelve la suma de los salarios de los empleados en el departamento de Ventas.

- **AVG:**

  Calcula el promedio de los valores en una columna.

  ```sql
  SELECT AVG(Edad)
  FROM Empleados;
  ```

  Devuelve la edad promedio de todos los empleados.

- **MIN y MAX:**

  MIN devuelve el valor mínimo en una columna.

  MAX devuelve el valor máximo en una columna.

  ```sql
  SELECT MIN(Salario), MAX(Salario)
  FROM Empleados;
  ```

  Devuelve el salario mínimo y máximo de todos los empleados.

- **GROUP BY:**

  Se utiliza junto con funciones de agregado para agrupar los resultados por una o más columnas.

  ```sql
  SELECT Departamento, AVG(Salario)
  FROM Empleados
  GROUP BY Departamento;
  ```

  Devuelve el salario promedio por departamento.

- **HAVING:**

  Se utiliza para filtrar los resultados de una cláusula GROUP BY basándose en una condición.

  ```sql
  SELECT Departamento, AVG(Salario)
  FROM Empleados
  GROUP BY Departamento
  HAVING AVG(Salario) > 50000;
  ```

## Instalación de MySql en Windows

Nos dirigimos a la siguiente pagina https://dev.mysql.com/downloads/windows/installer/8.0.html

<img align="center" src="/img/3ºimagenn.PNG"  />

Si por un casual la pagina no funcionara y estamos en la pagina oficial hemos de seleccionar esta versión.

Una vez descargado ejecutamos el archivo y procedemos a lo siguiente.

<img align="center" src="/img/4ºimagenn.PNG"  />

Seleccionamos la instalaccion completa y procedemos a descargar todos los paquetes, si nos diera error en la descargar procederemos a repetirla hasta que se descargen todos.

<img align="center" src="/img/5ºimagenn.PNG"  />

Tras esto los instalamos:

<img align="center" src="/img/6ºimagenn.PNG"  />

Procedemos a la configuracion de los paquetes:

<img align="center" src="/img/7ºimagenn.PNG"  />

<img align="center" src="/img/8ºimagenn.PNG"  />

Seleccionamos el método de autenticación, seleccionamos este y presionamos next, después se nos pedirá una contraseña para el usuario root.

<img align="center" src="C:\Users\Ramon\Repos git\DatabaseFundamentals\README\9ºimagenn-1709818348869-2.PNG"  /><img align="center" src="/img/10ºimagenn.PNG"  />

Dejamos la siguiente pestaña tal cual esta y clicamos next, tras esto clicamos en la siguiente opción para los permisos de los archivos del server.

<img align="center" src="C:\Users\Ramon\Repos git\DatabaseFundamentals\README\11ºimagenn.PNG"  /><img align="center" src="/img/12ºimagenn.PNG"  />

Después de esto ejecutamos para aplicar la configuración, durante este proceso se ira mostrando el avance, y tras finalizar pulsaremos finish.

<img align="center" src="/img/13ºimagenn.PNG"  />

Ahora procederemos con la configuración: 

<img align="center" src="C:\Users\Ramon\Repos git\DatabaseFundamentals\README\14ºimagenn.PNG"  />

Introduciremos la contraseña para comprobar la conexión, next, volveremos a presionar execute tras esto y clicaremos en finish.

<img align="center" src="/img/15ºimagenn.PNG"  />

Con esto ya estaría la instalación finalizada.

## Ejercicios SQL

Vamos a realizar el ejercico con un script proporcionado en el curso de Fundaula, entramos al Workbench de SQL introduciendo la clave root que escribimos al principio

<img align="center" src="/img/16ºimagenn.PNG"  />

Abrimos el script y lo ejecutamos desde File > Open SQL script cuando veamos el codigo ejecutamos dándole al boton del rayo

<img align="center" src="/img/17ºimagenn.PNG"  />

Tras esto vamos a Schemas actualizamos y deberiamos de ver lo siguiente:

<img align="center" src="/img/18ºimagenn.PNG"  />

Para empezar a trabajar en nuestra base de datos hemos de usar el siguiente comando y ejecutarlo con el botón de rayo:

```sql
use rentingsdb2;
```

<img align="center" src="/img/19ºimagenn.PNG"  />

### Ejercicio 1: Creación de una tabla.

Hemos de ejecutar el siguiente comando:

```sql
create table alquileres (
`alquilerID` int(5) not null auto_increment,
`clienteId` int(5) not null,
`cocheId` int(4) not null,
`seguroId` int(3) not null,
primary key (alquilerId)
);
```



Le damos la propiedad de autoincremento al id del alquiler que será nuestro primary key

### Ejercicio 2: Insertar datos en nuestra tabla.

Inicializamos la consulta de la tabla para ver que se encuentra vacía clicando en el siguiente icono:



<img align="center" src="C:\Users\Ramon\Repos git\DatabaseFundamentals\README\20ºimagenn.PNG"  /><img align="center" src="/img/21ºimagenn.PNG"  />

Abrimos un nuevo archivo sql y empezamos a introducir los distintos inserts:

Podemos introducirlo uno a uno e ir ejecutando uno a uno o escribirlos todos juntos y ejecutarlo en un solo archivo

```sql
insert	into alquileres
(alquilerId, clienteId, cocheId, seguroId)
values (1,4,2,1);

insert	into alquileres
(alquilerId, clienteId, cocheId, seguroId)
values (2,2,3,1);

insert	into alquileres
(alquilerId, clienteId, cocheId, seguroId)
values (3,1,5,2);
 
insert	into alquileres
(alquilerId, clienteId, cocheId, seguroId)
values (4,3,1,1);

insert	into alquileres
(alquilerId, clienteId, cocheId, seguroId)
values (5,5,4,2);
```

Comprobamos que los datos estén correctos volviendo a consultar la tabla 

<img align="center" src="/img/22ºimagenn.PNG"  />

### Ejercicio 3: Añadir columnas.

Usamos el comando alter para añadir las 2 nuevas columnas.

```sql
alter table alquileres
add column diasRenting  int(3) not null,
add column precio int(6) not null;

```

Comprobamos que se hayan creado consultando la tabla, se puede mirar también en la pestaña de información.

<img align="center" src="/img/23ºimagenn.PNG"  />

### Ejercicio 4: Actualizar y eliminar valores con update y delete

Lanzamos el comando update sobre la tabla de alquileres para los valores de cada columna y le indicamos que registro queremos modificar ya que si lo dejamos vacío modificaría todos los registros de la tabla con estos valores usando el where, procedemos a ejecutar y comprobamos

```sql
update alquileres
set diasRenting=8, precio=180
where alquilerId=1;
```

<img align="center" src="/img/24ºimagenn.PNG"  />

Seguimos rellenando la tabla, lo podemos hacer uno a uno o todos en comun:

```sql
update alquileres
set diasRenting=5, precio=145
where alquilerId=2;

update alquileres
set diasRenting=3, precio=170
where alquilerId=3;

update alquileres
set diasRenting=5, precio=195
where alquilerId=4;

update alquileres
set diasRenting=7, precio=260
where alquilerId=5;
```

Volvemos a consultar que todos los datos esten correctos y actualizados

<img align="center" src="/img/25ºimagenn.PNG"  />

Ahora vamos a proceder a eliminar los datos del alquilerID 2

```sql
delete from alquileres
where alquilerId=2;
```

<img align="center" src="/img/26ºimagenn.PNG"  />

Como podemos ver se borraron los valores.

### Ejercicio 5: Consulta de datos

Creamos un nuevo archivo y comenzamos usando el comando select, hemos de indicar que fila queremos obtener dentro de la tabla coches

```sql
select marca from coches;
```

<img align="center" src="/img/27ºimagenn.PNG"  />

Ahora hemos de usar distinct para obtener valores únicos dentro de la consulta, es decir no nos saldran valores repetidos

```sql
select distinct marca from coches;
```

<img align="center" src="/img/28ºimagenn.PNG"  />

Para poder filtrar tenemos el comando where que se usa de la siguiente manera si queremos por ejemplo obtener los alquileres con precio mayor a 185

```sql
select * from alquileres
where precio > 185;
```

El asterisco indica que escogemos todas las columnas de la tabla.

<img align="center" src="/img/29ºimagenn.PNG"  />



Ahora vamos a filtrar entre un rango con el comando between para mostrar por ejemplo todas las columnas donde los días de renting estén entre 3 y 7.

```sql
select * from alquileres
where diasRenting between 3 and 7;
```

<img align="center" src="/img/30ºimagenn.PNG"  />



Ahora vamos a filtrar los coches de la marca Audi con precio/día superior a 30, dentro de la tabla, haciendo la consulta ejecutamos lo siguiente.

```sql
SELECT * FROM rentingsdb2.coches;

select * from coches
where marca = 'Audi' and precioDia >30;
```

<img align="center" src="/img/31ºimagenn.PNG"  />

Ahora vamos a hacer el uso de ORDERBY que nos permite ordenar, vamos a ir a consultar la tabla de clientes y ordenarlos por apellidos en orden alfabético.

```sql
SELECT * FROM rentingsdb2.clientes;
select * from clientes
order by apellido asc;
```

<img align="center" src="/img/32ºimagenn.PNG"  />

Si queremos limitarlo a que nos de tan solo dos resultados usaremos limit de la siguiente manera

```sql
SELECT * FROM rentingsdb2.clientes;
select * from clientes
order by apellido asc
limit 2;

```

<img align="center" src="/img/34ºimagenn.PNG"  />



### Ejercicio 6: Uso del count.

Vamos a indicar cuantos clientes tenemos en nuestra tabla de clientes, para ello consultamos la tabla e introducimos el siguiente comando.

```sql
select	count(*)
from clientes;
```

<img align="center" src="/img/36ºimagenn.PNG"  />

Ahora vamos a indicar cuantos alquileres tenemos con un precio total de menos de 150:

```sql
select count(*)
from alquileres
where precio<150;
```

<img align="center" src="/img/37ºimagenn.PNG"  />

Lo comprobamos consultando la tabla de alquileres, efectivamente no hay ninguno

<img align="center" src="/img/38ºimagenn.PNG"  />

### Ejercicio 7: Uso del sum

Vamos a usar el  para indicar el total de los precios para ello usaremos sum de la siguiente manera:

```sql
select sum(precio) from alquileres;
```

Hay que tener en cuenta que tenemos que indicarle de que columna queremos la suma de la tabla de alquileres.

<img align="center" src="/img/39ºimagenn.PNG"  />



### Ejercicio 8: Uso del max y min

Vamos a indicar el precio máximo y mínimo de los alquileres de la siguiente manera:

Para mostrar el máximo:

```sql
select max(precio) from alquileres;
```

<img align="center" src="/img/40ºimagenn.PNG"  />

Para mostrar el minimo:

```sql
select min(precio) from alquileres;
```

<img align="center" src="/img/41ºimagenn.PNG"  />

Podemos comprobarlo con la imagen de la tabla de alquileres que tenemos en el ejercicio superior.

### Ejercicio 9: Uso del avg

Vamos a usar avg para calcular la media de días que se alquilan los coches.

```sql
select avg(diasRenting) from alquileres;
```

<img align="center" src="/img/43ºimagenn.PNG"  />

Podemos ver que el resultado nos sale con decimales, este resultado se puede redondear con la funcion ROUND



```sql
select round(avg(diasRenting),0) from alquileres;
```

Como podemos ver anidamos una funcion dentro de otra y como segundo parametro de la funcion round le indicamos el numero de decimales que queremos mostrar, donde 0 mostrara 0 decimales.

<img align="center" src="/img/42ºimagenn.PNG"  />
