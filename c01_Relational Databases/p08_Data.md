# Lección: Tipos de Datos y Almacenamiento en Bases de Datos

---

## 1. Introducción a los Datos
**Duración:** 00:00 - 00:10

¡Bienvenido a la última parte del capítulo sobre bases de datos! Esta lección se centrará en los datos dentro de una base de datos y su almacenamiento.

---

## 2. Tipos de Datos en SQL
**Duración:** 00:10 - 00:48

Cuando se crea una tabla, se debe indicar un tipo de dato para cada campo. El tipo de dato se elige en función del tipo de información que contendrá el campo, como números, texto o fechas. Los tipos de datos son importantes por varias razones:
1. Diferentes tipos de datos se almacenan de forma distinta y ocupan diferentes cantidades de espacio.
2. Algunas operaciones solo son aplicables a ciertos tipos de datos. Por ejemplo, tiene sentido multiplicar un número por otro, pero no tiene sentido multiplicar texto.

---

## 3. Strings
**Duración:** 00:48 - 01:36

En programación, un **string** (cadena) es una secuencia de caracteres como letras o puntuación. En la tabla **patrons**, los datos en el campo **names** están compuestos de strings, como "Maham" y "James". SQL tiene varios tipos de datos para almacenar strings:
- Algunas cadenas pueden ser cortas (hasta 250 caracteres), lo que ahorra espacio de almacenamiento.
- El tipo de dato **VARCHAR** es flexible y puede almacenar cadenas pequeñas o grandes (hasta decenas de miles de caracteres). Debido a su flexibilidad, **VARCHAR** es muy utilizado para almacenar strings.

---

## 4. Enteros (Integers)
**Duración:** 01:36 - 02:03

Los tipos de datos de enteros almacenan números enteros, como los años en la columna **member_year** de la tabla **patrons**. SQL ofrece varios tipos de datos de enteros, dependiendo del tamaño de los números que queremos almacenar. Por ejemplo, el tipo de dato **INT** puede almacenar números desde menos de dos mil millones negativos hasta más de dos mil millones positivos.

---

## 5. Flotantes (Floats)
**Duración:** 02:03 - 02:33

Los tipos de datos de números flotantes almacenan números con parte decimal, como los 2.05 dólares que Jasmin debe en multas. SQL también ofrece varios tipos de datos para flotantes, dependiendo de cuántos dígitos se esperan antes y después del punto decimal. El tipo de dato **NUMERIC** puede almacenar flotantes con hasta 38 dígitos en total.

---

## 6. Esquemas de Bases de Datos
**Duración:** 02:33 - 03:12

Ahora que conocemos los tipos de datos, podemos analizar un **esquema de base de datos**. Un esquema se describe como el "plano" de una base de datos. Muestra el diseño de la base de datos, como las tablas incluidas y las relaciones entre ellas. También indica qué tipo de dato puede contener cada campo. En el esquema de nuestra base de datos de la biblioteca, el tipo de dato **VARCHAR** se utiliza para strings como el título del libro, autor y género. También podemos ver que la tabla **patrons** está relacionada con la tabla **checkouts**, pero no con la tabla **books**.

---

## 7. Almacenamiento en Bases de Datos
**Duración:** 03:12 - 03:53

Finalmente, discutamos el almacenamiento. La información que encontramos en una tabla de base de datos se almacena físicamente en el disco duro de un **servidor**. Los servidores son computadoras centralizadas que realizan servicios mediante solicitudes a través de una red. En nuestro caso, el servicio es el acceso a datos, pero los servidores también se utilizan para acceder a sitios web o archivos almacenados en el servidor. Cualquier computadora puede ser un servidor si está configurada para proporcionar un servicio, incluso una laptop. Sin embargo, los servidores suelen ser máquinas potentes y grandes, porque están equipadas para manejar un gran volumen de solicitudes y datos.

---

## 8. ¡A Practicar!
**Duración:** 03:53 - 03:59

¡Bien, pongamos en práctica lo aprendido sobre los datos!