## **Ejercicio: Creando una Vista en SQL**

### **Descripción del Ejercicio:**

En este ejercicio, vas a guardar el resultado de una consulta en una **vista**. Una **vista** en SQL es una tabla virtual que no almacena los datos, sino que guarda el código de una consulta que genera un resultado. La ventaja de una vista es que cuando los datos en las tablas originales cambian, los resultados de la vista también se actualizan, ya que se vuelve a ejecutar la consulta.

---

### **Instrucciones: Guardar los Resultados de una Consulta como una Vista**

En el código presentado, hemos escrito una consulta que selecciona autores únicos y les asigna un alias `unique_author`. Ahora, vamos a guardar esa consulta como una vista llamada `library_authors`, para que pueda ser consultada en el futuro sin necesidad de escribir la misma consulta de nuevo.

#### **Consulta SQL para Crear una Vista:**
```sql
-- Guardar los resultados de la consulta como una vista llamada library_authors
CREATE VIEW library_authors AS
SELECT DISTINCT author AS unique_author
FROM books;
```

- **Explicación**:
   - **CREATE VIEW library_authors AS**: Esta línea crea una vista llamada `library_authors`. La vista es el resultado de la consulta que viene después.
   - **SELECT DISTINCT author AS unique_author**: Esta es la consulta que selecciona autores únicos de la tabla `books` y les asigna el alias `unique_author`.
   - **FROM books**: La consulta selecciona los datos de la tabla **books**.

El código crea una vista llamada `library_authors`, que genera una lista de autores únicos cada vez que es consultada. La vista no almacena datos físicamente, solo guarda la consulta.

---

### **¿Qué es una Vista?**

- **Tabla Virtual**: Una vista es como una tabla, pero no almacena datos. Al acceder a la vista, lo que realmente sucede es que la consulta guardada se ejecuta de nuevo, mostrando los datos actualizados.
- **Reutilización de Consultas**: Una vez creada la vista, puedes utilizarla como cualquier tabla real en otras consultas SQL. Esto te ahorra tiempo al evitar que tengas que reescribir consultas largas o complejas.
- **Actualización Dinámica**: Como la vista no guarda los datos de manera física, cada vez que se consulta la vista, los datos reflejan los cambios más recientes de las tablas de origen.

---

### **Conclusión**:

Las vistas son herramientas muy útiles en SQL para guardar consultas y reutilizarlas fácilmente. Al crear una vista, puedes evitar escribir la misma consulta repetidamente y asegurarte de que siempre estás trabajando con los datos más actualizados de las tablas originales.