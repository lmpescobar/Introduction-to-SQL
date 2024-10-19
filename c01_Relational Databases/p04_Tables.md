# Lección: Tablas en Bases de Datos

---

## 1. Introducción a las Tablas
**Duración:** 00:00 - 00:09

Ahora que conocemos la organización básica de una base de datos, veamos de cerca el bloque principal de construcción de las bases de datos: ¡las tablas!

---

## 2. Organización de las Tablas
**Duración:** 00:09 - 00:38

En la lección anterior vimos que las bases de datos se organizan en tablas, las cuales contienen datos relacionados sobre un tema particular. Como hemos observado, las tablas están organizadas en filas y columnas; en el mundo de las bases de datos, las filas a menudo se denominan **registros** y las columnas como **campos**. Los campos de una tabla están limitados a los definidos cuando la base de datos fue creada, pero el número de filas es ilimitado.

---

## 3. Buenas Prácticas en el Nombrado de Tablas
**Duración:** 00:38 - 01:00

Hablemos un poco sobre el nombrado de las tablas. Los nombres de las tablas deben estar en minúsculas y no deben contener espacios; en su lugar, se utilizan guiones bajos. Idealmente, un nombre de tabla debe referirse a un grupo colectivo (como "inventario"), pero también está bien que el nombre de la tabla sea plural (como "productos").

---

## 4. Registros de la Tabla
**Duración:** 01:00 - 01:24

Un **registro** es una fila en una tabla. Contiene datos sobre una observación individual. Si observamos la tabla de usuarios de la biblioteca, podemos ver que tiene cuatro registros: uno para cada usuario. El registro de Jasmin indica que se hizo miembro en 2022 y debe dos dólares con cinco centavos en multas.

---

## 5. Campos de la Tabla
**Duración:** 01:24 - 01:38

Un **campo** es una columna en una tabla. Contiene una pieza de información sobre todas las observaciones en la tabla. El campo "nombre" en la tabla de usuarios de la biblioteca enumera los nombres de todos los usuarios.

---

## 6. Más Buenas Prácticas para el Nombrado de Campos
**Duración:** 01:38 - 02:21

Debido a que los nombres de los campos deben ser escritos al consultar una base de datos con SQL, el nombrado de los campos es importante. Generalmente, los nombres de los campos deben estar en minúsculas y no deben contener espacios. Un nombre de campo debe ser singular en lugar de plural, ya que se refiere a la información contenida en ese campo para un solo registro. Por esta razón, nuestra tabla tiene los campos "card_num" y "name" en lugar de "card_nums" y "names". Además, dos campos en una tabla no pueden tener el mismo nombre, y los nombres de los campos no deben compartir un nombre con la tabla en la que se encuentran, para evitar confusión al referirse a un campo o una tabla.

---

## 7. Identificadores Únicos
**Duración:** 02:21 - 02:49

Un **identificador único**, a veces llamado "clave", es exactamente lo que parece: un valor único que identifica un registro para distinguirlo de otros registros en la misma tabla. Este valor, con frecuencia, es un número. En la tabla de usuarios, tiene sentido usar el campo "card_num" como el identificador único para cada usuario, en lugar del campo "nombre", ya que es posible que dos usuarios tengan el mismo nombre a medida que crezca nuestra biblioteca.

---

## 8. Mejor con Más Tablas
**Duración:** 02:49 - 03:36

Tener más tablas, cada una con un tema claramente definido, generalmente es mejor que tener menos tablas donde se combine información sobre varios temas. Observa las tablas de usuarios y préstamos. Ahora, aquí está cómo se verían nuestras tablas si intentáramos combinarlas. Es la misma información, pero mucho menos clara, ya que contiene información duplicada. Aunque podemos ver que Izzy tiene dos préstamos y Maham no tiene ninguno, la columna "card_num" ya no es única debido a los múltiples préstamos de Izzy. Siempre podemos usar SQL para obtener información de varias tablas relacionadas y conectarlas si es necesario, pero los temas de las tablas deben permanecer separados.

---

## 9. ¡A Practicar!
**Duración:** 03:36 - 03:42

¡Pongamos en práctica todo lo aprendido sobre las tablas con algunos ejercicios!