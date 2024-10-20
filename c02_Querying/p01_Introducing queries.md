# Masterclass: Introducción a las Consultas SQL

---

### 1. Introducción a las consultas SQL
Las consultas SQL permiten extraer información significativa de bases de datos de manera eficiente. Una vez que se comprende cómo está organizada la información en una base de datos, se puede comenzar a realizar consultas para obtener respuestas específicas a partir de los datos almacenados. SQL es el lenguaje utilizado para interactuar con las bases de datos relacionales, facilitando la extracción y análisis de datos.

---

### 2. Utilidad de SQL
SQL es extremadamente útil para responder preguntas tanto dentro de una tabla como entre varias tablas en bases de datos relacionales. Por ejemplo, en una base de datos de una biblioteca, SQL puede utilizarse para encontrar qué libros ha tomado prestados un usuario en un año determinado. En una base de datos de recursos humanos, SQL podría emplearse para comparar los salarios de empleados en distintos departamentos, como Marketing y Contabilidad, para verificar si los pagos son equitativos. SQL es capaz de manejar estos escenarios de consulta y muchos más, permitiendo obtener información precisa a partir de datos complejos.

---

### 3. SQL y grandes volúmenes de datos
SQL es especialmente potente cuando se trabaja con grandes volúmenes de datos. Aunque herramientas como las hojas de cálculo son útiles para conjuntos de datos pequeños o simples, cuando los datos tienen múltiples relaciones o cuando el volumen es considerable, el uso de bases de datos relacionales y SQL se vuelve esencial. Por ejemplo, en plataformas de comercio electrónico, SQL permite organizar y analizar datos masivos sobre tráfico web, opiniones de clientes y ventas de productos. Las consultas SQL pueden responder preguntas como "¿Qué productos tuvieron más ventas la semana pasada?" o "¿Qué productos recibieron las peores calificaciones de los clientes?" SQL es una herramienta imprescindible cuando se trata de gestionar y analizar grandes cantidades de datos con relaciones complejas.

---

### 4. Palabras clave en SQL
Para escribir código SQL, es fundamental entender las palabras clave que se utilizan para indicar las operaciones a realizar. Dos de las palabras clave más comunes son `SELECT` y `FROM`. `SELECT` se utiliza para especificar qué campos o columnas se desean extraer de una tabla, mientras que `FROM` se utiliza para indicar de qué tabla se obtendrán esos campos. Por ejemplo, si se necesita una lista con los nombres de los usuarios de una biblioteca, se utilizaría `SELECT` seguido del campo `name`, y `FROM` seguido del nombre de la tabla, como `patrons`. Estas palabras clave son fundamentales para empezar a escribir consultas SQL.

---

### 5. Nuestra primera consulta
Para escribir una consulta básica, el comando `SELECT` se coloca primero, seguido por `FROM`. La consulta se cierra generalmente con un punto y coma (`;`) para indicar que ha finalizado. Es una buena práctica escribir las palabras clave en mayúsculas (como `SELECT` y `FROM`), mientras que los nombres de las tablas y campos se escriben en minúsculas. El resultado de la consulta, conocido como "conjunto de resultados" o "result set", mostrará los datos solicitados. Cabe destacar que, al realizar consultas, la base de datos no se modifica; simplemente se obtienen los datos en función de los criterios establecidos en la consulta. Los resultados obtenidos pueden compartirse guardando el código SQL para que otros puedan ejecutar la misma consulta en el futuro.

---

### 6. Selección de múltiples campos
Si se desea seleccionar más de un campo de una tabla, es posible hacerlo listando varios nombres de campos separados por comas después de la palabra clave `SELECT`. Por ejemplo, si se desea obtener tanto el número de tarjeta como el nombre de los usuarios, se listarán ambos campos en el orden en que se deseen en los resultados. El orden en el que se listan los campos en la consulta no tiene que coincidir con el orden en el que aparecen en la tabla.

---

### 7. Selección de múltiples campos (continuación)
De la misma manera que se pueden seleccionar dos campos, también es posible seleccionar tres o más campos. Por ejemplo, si se desea obtener el nombre, el número de tarjeta y el total de multas de un usuario, simplemente se listan estos tres campos en la consulta, separados por comas.

---

### 8. Selección de todos los campos
Si se necesita seleccionar todos los campos de una tabla, en lugar de listar cada uno de ellos, es posible usar un asterisco (`*`) después de `SELECT`. El asterisco le indica a SQL que debe recuperar todos los campos de la tabla. Esto simplifica la consulta cuando se desean obtener todos los datos disponibles sin tener que especificar cada campo de manera individual.

---

### 9. Práctica
Una vez entendidos estos conceptos básicos de SQL, es importante practicar escribiendo consultas. En el siguiente ejercicio, se trabajará con la tabla de libros presentada en el capítulo anterior. Esta tabla contiene 350 libros que forman parte del catálogo de la biblioteca. Practicar la escritura de consultas permite familiarizarse con la sintaxis y los conceptos fundamentales del lenguaje SQL, preparándote para abordar escenarios más complejos en el futuro.


En resumen, SQL es una herramienta poderosa para obtener información precisa de grandes volúmenes de datos organizados en bases de datos relacionales. A través de consultas bien formuladas, es posible analizar información de manera eficiente, respondiendo a preguntas clave que son difíciles de resolver con herramientas más simples como las hojas de cálculo. Practicar la escritura de consultas es esencial para dominar este lenguaje y aprovechar al máximo su potencial.