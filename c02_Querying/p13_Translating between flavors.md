### Ejercicio: Traduciendo entre versiones (flavors) de SQL

### Descripción:
Este ejercicio se enfoca en cómo traducir consultas SQL entre diferentes versiones o "flavors" de SQL. En particular, la tarea consiste en convertir una consulta escrita en PostgreSQL para que funcione en SQL Server. Cada **flavor** de SQL tiene pequeñas diferencias en cuanto a la sintaxis, y en este caso nos centraremos en el uso de la palabra clave **LIMIT** en PostgreSQL y cómo traducirla a **TOP** en SQL Server.

### Consulta Original en PostgreSQL:
```sql
SELECT genre
FROM books
LIMIT 10;
```

La consulta anterior selecciona el campo **genre** de la tabla **books** y limita los resultados a 10 filas usando la palabra clave **LIMIT**.

### Pregunta:
¿Cómo traducirías esta consulta para que funcione en SQL Server?

---

### Opciones y Explicación:

1. **Opción 1: Reemplazar FROM con TABLE**
   - Esta opción es incorrecta. El uso de **FROM** es estándar en ambas versiones de SQL, por lo que no hay necesidad de reemplazarlo con **TABLE**.

2. **Opción 2: Reemplazar SELECT, FROM y LIMIT con las palabras clave correspondientes en SQL Server**
   - Aunque SQL Server tiene su propio "flavor", no se necesita reemplazar **SELECT** y **FROM** porque son iguales en ambas versiones. Solo la palabra **LIMIT** necesita ser ajustada.

3. **Opción 3: Eliminar LIMIT y agregar TOP(10) después de SELECT**
   - **Correcto.** SQL Server no utiliza **LIMIT**; en su lugar, utiliza **TOP(n)** para limitar el número de resultados. La traducción correcta sería:
   ```sql
   SELECT TOP(10) genre
   FROM books;
   ```
   - Aquí, **TOP(10)** limita el número de resultados a 10, como lo hacía **LIMIT** en PostgreSQL.

4. **Opción 4: Reemplazar LIMIT con TOP y eliminar el punto y coma al final de la consulta**
   - Esta opción es incorrecta, ya que el punto y coma es opcional y no tiene un impacto en la sintaxis de la consulta en SQL Server. Además, no es necesario eliminar el punto y coma para que la consulta funcione.

### Conclusión:
Para traducir la consulta de PostgreSQL a SQL Server, solo necesitamos reemplazar **LIMIT** con **TOP(n)** y dejar el resto de la consulta igual.