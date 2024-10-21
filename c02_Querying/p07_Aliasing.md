## **Ejercicio: Uso de Alias en SQL**

### **Descripción del Ejercicio:**

En este ejercicio, aprenderás cómo usar **aliasing** para renombrar columnas en el resultado de una consulta SQL. Esto es útil cuando deseas que los resultados sean más claros, ya sea para hacer los nombres más breves o para proporcionar un contexto adicional sobre lo que contienen las columnas.

Un **alias** permite cambiar el nombre de una columna solo en el resultado de la consulta, sin modificar el nombre real de la columna en la tabla original. Esto es especialmente útil para mejorar la legibilidad de los resultados, especialmente cuando los nombres de las columnas originales no son lo suficientemente descriptivos.

---

### **Instrucción: Añadir un Alias al Campo `author`**

#### **Consulta SQL:**
```sql
SELECT DISTINCT author AS unique_author
FROM books;
```

- **Explicación**:
   - **SELECT DISTINCT**: Selecciona solo los valores únicos del campo especificado.
   - **author**: Este es el campo que contiene los nombres de los autores.
   - **AS unique_author**: Aquí estamos usando **AS** para asignar un alias, cambiando el nombre de la columna `author` en los resultados de la consulta por `unique_author`. Este alias solo afecta el resultado y no modifica el nombre de la columna en la tabla original.
   - **FROM books**: Selecciona los datos de la tabla **books**.

El resultado de la consulta mostrará una lista de autores únicos con la columna renombrada como `unique_author`.

---

### **Beneficios de Usar Alias:**

- **Claridad**: Renombrar las columnas hace que los resultados sean más fáciles de interpretar para los usuarios o colaboradores que puedan no estar familiarizados con los nombres de campo en la tabla original.
- **Brevity**: Usar alias puede acortar nombres de columnas largos y hacer que los resultados sean más fáciles de leer.
- **No afecta los datos originales**: El alias solo cambia el nombre de la columna en los resultados de la consulta, sin modificar la tabla original o los nombres de los campos en la base de datos.

---

### **Conclusión**:

El uso de aliasing en SQL es una forma efectiva de personalizar los resultados de una consulta, mejorando la legibilidad y comprensión de los datos sin alterar la estructura de la base de datos.