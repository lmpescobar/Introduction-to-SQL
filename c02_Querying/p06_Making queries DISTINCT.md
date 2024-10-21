## **Ejercicio: Usando DISTINCT en Consultas SQL**

### **Descripción del Ejercicio:**

Este ejercicio tiene como objetivo enseñarte cómo usar la palabra clave **DISTINCT** para devolver valores únicos en un campo de una tabla. En este caso, trabajamos con la tabla **books** que contiene un listado de 350 libros disponibles para préstamo en una biblioteca.

Aunque hay 350 libros, es probable que no haya 350 autores diferentes, ya que algunos de los autores habrán escrito varios libros. Por ejemplo, si la biblioteca tiene los siete libros de Harry Potter, todos fueron escritos por **J.K. Rowling**, por lo tanto, aparecerá varias veces en la tabla. El objetivo es aprender cómo extraer solo los valores únicos en estos casos.

---

### **Instrucción 1/2: Seleccionar autores únicos**

#### **Consulta SQL:**
```sql
SELECT DISTINCT author
FROM books;
```

- **Explicación**:
   - **DISTINCT**: Devuelve solo los valores únicos del campo especificado, eliminando los duplicados.
   - **author**: Este es el campo que contiene los nombres de los autores.
   - **FROM books**: Especifica que estamos seleccionando datos de la tabla **books**.
   - El resultado de esta consulta es un listado de autores únicos que están representados en la tabla de libros.

---

### **Instrucción 2/2: Seleccionar combinaciones únicas de autor y género**

#### **Consulta SQL:**
```sql
SELECT DISTINCT author, genre
FROM books;
```

- **Explicación**:
   - Aquí estamos usando **DISTINCT** para seleccionar combinaciones únicas de dos campos: `author` y `genre`. Esto significa que devolverá solo las combinaciones únicas de autor y género.
   - El resultado de esta consulta será una lista de combinaciones únicas donde cada autor estará asociado con un género de libro, eliminando las combinaciones repetidas.
  
---

### **Beneficios del uso de DISTINCT**:

- **Evitar duplicados**: Esta palabra clave es extremadamente útil cuando se necesita trabajar con valores únicos en grandes conjuntos de datos. En vez de tener resultados duplicados, **DISTINCT** garantiza que cada valor o combinación de valores aparezca solo una vez.
- **Aplicable a múltiples campos**: Como vimos en el segundo ejemplo, también es posible aplicar **DISTINCT** a más de un campo, lo que permite obtener combinaciones únicas de múltiples valores.
  
---

### **Conclusión**:

El uso de **DISTINCT** en SQL es una poderosa herramienta para limpiar los resultados y evitar duplicados. Ya sea que estés trabajando con un solo campo o combinaciones de varios campos, esta palabra clave te ayudará a obtener resultados más precisos y enfocados en lo que necesitas.