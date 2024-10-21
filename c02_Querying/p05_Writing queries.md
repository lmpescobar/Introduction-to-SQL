## Masterclass: Consultas Avanzadas en SQL

### **1. Introducción a las consultas avanzadas**
Para llevar nuestras consultas SQL al siguiente nivel, es fundamental aprender algunas palabras clave que se usan comúnmente. Estas palabras clave nos permiten manejar los datos de manera más precisa y eficiente. Vamos a profundizar en estos conceptos.

---

### **2. Alias en SQL (Aliasing)**

A veces, es útil renombrar las columnas en nuestro conjunto de resultados para mayor claridad o brevedad. Esta técnica se conoce como **aliasing** y se realiza mediante la palabra clave `AS`. 

Por ejemplo, si queremos seleccionar el nombre y el año de contratación de cada empleado en la tabla **employees**, podemos hacer lo siguiente:

```sql
SELECT name AS first_name, year_hired
FROM employees;
```

- **Explicación**: Aquí hemos renombrado la columna `name` a `first_name`. Esto afecta solo al conjunto de resultados, no a los nombres de las columnas en la tabla original.

- **Importante**: El alias es temporal y solo aplica a la consulta actual. La columna en la tabla original sigue manteniendo su nombre original, en este caso, `name`.

---

### **3. Seleccionar registros únicos (DISTINCT)**

En algunas consultas SQL, es útil devolver solo los valores únicos de una columna. Esto se logra con la palabra clave **DISTINCT**.

Por ejemplo, si queremos obtener una lista de años de contratación sin repeticiones en la tabla **employees**:

```sql
SELECT DISTINCT year_hired
FROM employees;
```

- **Explicación**: En este caso, SQL devolverá solo los años de contratación únicos. Si varios empleados fueron contratados el mismo año, ese año solo aparecerá una vez en los resultados.

Este enfoque es ideal cuando necesitamos eliminar duplicados y trabajar solo con valores únicos.

---

### **4. Usar DISTINCT con múltiples campos**

El uso de **DISTINCT** no está limitado a una sola columna; también podemos aplicarlo a múltiples campos. Esto nos permite obtener combinaciones únicas de varios valores.

Por ejemplo, si deseamos ver los años en que diferentes departamentos contrataron empleados:

```sql
SELECT DISTINCT dept_id, year_hired
FROM employees;
```

- **Explicación**: Esta consulta devolverá combinaciones únicas de departamentos y años de contratación. Por ejemplo, si el departamento 3 contrató a dos empleados en 2021, solo aparecerá una vez esa combinación en los resultados.

---

### **5. Combinaciones únicas con DISTINCT**

Incluso cuando usamos **DISTINCT** en varias columnas, es posible que los valores individuales de las columnas se repitan, pero lo importante es que la combinación de esas columnas será única.

Por ejemplo:
- En los resultados puede que veamos `dept_id` 3 repetido, o el año `2021`, pero nunca en la misma combinación exacta de ambos valores.

---

### **6. Vistas en SQL (Views)**

En SQL, una **vista** es una tabla "virtual" que se crea a partir de una consulta SQL guardada. A diferencia de una tabla real, los datos de una vista no se almacenan físicamente en la base de datos. En su lugar, la consulta que genera esos datos se almacena, y cada vez que accedemos a la vista, la consulta se ejecuta y devuelve datos actualizados.

Para crear una vista:

```sql
CREATE VIEW employee_hire_years AS
SELECT name, dept_id, year_hired
FROM employees;
```

- **Explicación**: En este caso, hemos creado una vista llamada `employee_hire_years`, que selecciona los campos `name`, `dept_id` y `year_hired` de la tabla **employees**. Cuando accedemos a esta vista en el futuro, los resultados reflejarán cualquier actualización en la tabla subyacente.

---

### **7. Usar vistas**

Una vez que una vista ha sido creada, podemos consultarla como si fuera una tabla normal. Por ejemplo, para obtener datos de la vista `employee_hire_years`, usaríamos la siguiente consulta:

```sql
SELECT *
FROM employee_hire_years;
```

- **Explicación**: Aquí estamos seleccionando todos los campos de la vista que creamos previamente. Al ser una vista, siempre estará actualizada con los últimos datos de la tabla subyacente.

---

### **8. Práctica**

Ahora que conocemos estas nuevas palabras clave como **DISTINCT**, **AS** (alias) y **CREATE VIEW**, es hora de practicar. Estos conceptos son fundamentales para realizar consultas más complejas y optimizar el manejo de grandes volúmenes de datos.

---

## **Conclusión**

- **Alias** (`AS`) nos permite renombrar columnas de manera temporal en nuestros resultados.
- **DISTINCT** nos permite eliminar duplicados y obtener solo valores únicos, ya sea de una columna o de una combinación de varias columnas.
- **Vistas** nos permiten guardar consultas como tablas virtuales para un acceso fácil y eficiente a los datos actualizados.