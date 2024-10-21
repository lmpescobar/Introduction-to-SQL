## **Ejercicio: Crear y Consultar una Vista en SQL**

### **Descripción del Ejercicio:**

Este ejercicio tiene como objetivo aprender cómo **crear una vista** en SQL y luego **consultarla**. Una vista en SQL es una tabla virtual basada en el resultado de una consulta. En lugar de almacenar datos de forma física, almacena el código de la consulta que genera el resultado. 

Una vez que la vista ha sido creada, puedes consultarla como si fuera una tabla normal.

---

### **Instrucciones para Crear y Consultar la Vista:**

1. **Crear la Vista**:
   En el primer paso, debes crear una vista llamada `library_authors` que muestre los autores únicos de la tabla `books`. Aquí está el código para crear la vista:

```sql
-- Crear la vista library_authors
CREATE VIEW library_authors AS
SELECT DISTINCT author AS unique_author
FROM books;
```

- **Explicación**:
   - **CREATE VIEW library_authors AS**: Esta línea crea una vista llamada `library_authors`.
   - **SELECT DISTINCT author AS unique_author**: Aquí seleccionamos autores únicos de la tabla `books` y les asignamos un alias `unique_author`.
   - **FROM books**: Los datos son extraídos de la tabla `books`.

---

2. **Consultar la Vista**:
   Después de haber creado la vista, podemos consultarla para verificar que ha sido creada correctamente y que devuelve los datos esperados. Para hacer esto, selecciona todas las columnas de la vista `library_authors`:

```sql
-- Consultar todas las columnas de la vista library_authors
SELECT *
FROM library_authors;
```

- **Explicación**:
   - **SELECT \***: Seleccionamos todas las columnas de la vista `library_authors`.
   - **FROM library_authors**: La consulta extrae los datos de la vista creada anteriormente.

---

### **Conclusión:**

Las vistas son muy útiles cuando necesitas reutilizar consultas complejas o generar resultados dinámicos que siempre estén actualizados según los datos en las tablas de origen. En este ejercicio, aprendiste cómo crear una vista y consultarla, aprovechando la funcionalidad que ofrece SQL para organizar y acceder a datos de manera eficiente.