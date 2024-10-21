# Ejercicio: Desarrollando Estilo en SQL

### Descripción:
Es importante prestar atención al **formato de las consultas SQL** para que sean legibles y fáciles de entender. Esto es especialmente útil a medida que se aprenden más palabras clave y las consultas se vuelven más largas.

En este ejercicio, se revisa una consulta SQL sobre la tabla **patrons**. El código funcionará correctamente, pero está desordenado y es difícil de leer. La tarea consiste en determinar qué ediciones son apropiadas para mejorar el estilo de la consulta, siguiendo las mejores prácticas de estilo en SQL.

---

### Consulta SQL a Revisar:
```sql
SELECT CARD_NUM, TOTAL_FINE
FROM patrons
```

---

### Tabla `patrons`:

| card_num | name   | member_year | total_fine |
|----------|--------|-------------|------------|
| 54378    | Izzy   | 2012        | 9.86       |
| 94722    | Maham  | 2020        | 0          |
| 45783    | Jasmin | 2022        | 2.05       |
| 90123    | James  | 1989        | 0          |

---

## Instrucciones:

Arrastra cada sugerencia a la zona correcta dependiendo de si mejorará el estilo de la consulta.

---

## Sugerencias para mejorar el estilo:

1. **Hacer que `CARD_NUM` y `TOTAL_FINE` estén en minúsculas**:

   - Según las mejores prácticas, los nombres de los campos deben estar en minúsculas para mejorar la legibilidad y seguir un formato coherente.

2. **Capitalizar `FROM`**:

   - Las palabras clave en SQL, como `SELECT` y `FROM`, deben estar en mayúsculas para destacarse del resto del código.

3. **Agregar un punto y coma (`;`) al final de la consulta**:

   - Terminar la consulta con un punto y coma es una buena práctica para indicar que la consulta ha finalizado, lo cual es especialmente importante cuando se ejecutan múltiples consultas.

---

## Sugerencias que no mejoran el estilo:

1. **Capitalizar `patrons`**:

   - El nombre de la tabla debe estar en minúsculas, siguiendo las convenciones de estilo. No es necesario capitalizarlo.

2. **Todo el código debe estar en una sola línea**:

   - Dividir el código en varias líneas mejora la legibilidad, especialmente en consultas más largas. Mantenerlo en una sola línea no es recomendable.

3. **Hacer que `SELECT` esté en minúsculas**:

   - Las palabras clave como `SELECT` deben estar en mayúsculas para seguir las mejores prácticas de SQL y hacer que el código sea más fácil de leer y entender.

---

## Mejores Prácticas para Consultas SQL:

1. **Uso de mayúsculas en palabras clave**: Las palabras clave de SQL (como `SELECT`, `FROM`, `WHERE`) deben escribirse en mayúsculas para diferenciarlas claramente de los nombres de tablas y columnas.

2. **Minúsculas para nombres de tablas y campos**: Se recomienda usar minúsculas para los nombres de tablas y campos, ya que mejora la consistencia y hace que el código sea más legible.

3. **Punto y coma al final de las consultas**: Terminar cada consulta con un punto y coma (`;`) es una práctica estándar para evitar errores y garantizar que el código esté completo.

4. **Formato en varias líneas**: Escribir el código SQL en varias líneas mejora la legibilidad, especialmente en consultas más complejas que involucran múltiples tablas o condiciones.