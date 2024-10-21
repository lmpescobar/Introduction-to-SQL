### Ejercicio: Limitar resultados en SQL

### Descripción:
En este ejercicio, vamos a practicar cómo utilizar la cláusula **LIMIT** en SQL para restringir el número de resultados que obtenemos de una consulta. Este concepto es muy útil cuando se trabaja con bases de datos grandes que pueden devolver miles o incluso millones de resultados. Limitar los resultados ayuda a probar y depurar el código sin esperar grandes volúmenes de datos.

### Instrucciones del Ejercicio:
1. Usando PostgreSQL, selecciona el campo **genre** de la tabla **books**.
2. Limita el número de resultados a **10** utilizando la cláusula **LIMIT**.

---

### Consulta SQL proporcionada:
```sql
-- Seleccionar los primeros 10 géneros de la tabla books usando PostgreSQL
SELECT genre 
FROM books
LIMIT 10;
```

### Explicación del Código:

1. **SELECT genre**: Esta parte de la consulta indica que queremos seleccionar el campo **genre** de la tabla. El campo **genre** contiene los géneros de los libros en la base de datos.
   
2. **FROM books**: Aquí indicamos que los datos que queremos extraer provienen de la tabla **books**.

3. **LIMIT 10**: Esta cláusula es clave para el ejercicio. **LIMIT** le dice a la base de datos que solo devuelva un número específico de filas, en este caso, **10**. Esto significa que obtendremos solo los primeros 10 géneros disponibles en la tabla **books**, en lugar de todos los géneros que podrían ser cientos o miles.

### ¿Por qué es importante LIMIT?
El uso de **LIMIT** es muy común cuando trabajamos con grandes volúmenes de datos. En lugar de obtener todos los resultados de una tabla, que podría ser ineficiente y ralentizar el proceso, **LIMIT** permite obtener solo una pequeña porción de datos para probar las consultas, facilitando el trabajo de desarrollo y depuración.

Este enfoque es especialmente útil cuando se hacen cambios incrementales en las consultas y se necesita verificar rápidamente si están funcionando como se espera sin sobrecargar el sistema con grandes cantidades de datos.