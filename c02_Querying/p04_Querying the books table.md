## **Ejercicio: Consultar la tabla de libros**

### **Descripción:**
En este ejercicio, practicarás escribir tus primeras consultas SQL utilizando las palabras clave **SELECT** y **FROM**. Recuerda que **SELECT** se usa para elegir los campos que serán incluidos en el conjunto de resultados, mientras que **FROM** se utiliza para indicar de qué tabla se seleccionarán los campos.

Tienes la tabla **books** y el objetivo es practicar la selección de campos de dicha tabla.

---

### **Instrucciones 1/3:**

- **Usa SQL para devolver un conjunto de resultados con todos los títulos de los libros incluidos en la tabla `books`.**

#### Consulta:
```sql
-- Devuelve todos los títulos de la tabla books
SELECT *
FROM books;
```

#### **Explicación:**
- **SELECT**: Esta palabra clave selecciona las columnas que queremos ver en el conjunto de resultados. En este caso, al usar un asterisco (`*`), estamos diciendo que queremos seleccionar todas las columnas.
- **FROM**: Esta palabra clave especifica la tabla de la que estamos seleccionando los datos. En este caso, seleccionamos la tabla `books`.

**Resultado:** Muestra todas las columnas (id, title, author, etc.) de todos los libros en la tabla.

---

### **Instrucciones 2/3:**

- **Selecciona tanto los campos `title` como `author` de la tabla `books`.**

#### Consulta:
```sql
-- Selecciona los campos title y author de la tabla books
SELECT title, author
FROM books;
```

#### **Explicación:**
- **SELECT title, author**: En esta consulta estamos especificando que queremos seleccionar solo dos columnas de la tabla `books`: el título (`title`) y el autor (`author`).
- **FROM**: Indicamos de qué tabla se van a seleccionar estas columnas, que en este caso sigue siendo `books`.

**Resultado:** Solo se muestran las columnas de título y autor de cada libro.

**Pista:** Para seleccionar múltiples campos, coloca los nombres de los campos después de la palabra clave **SELECT** y sepáralos por una coma.

---

### **Instrucciones 3/3:**

- **Selecciona todos los campos de la tabla `books`.**

#### Consulta:
```sql
-- Selecciona todos los campos de la tabla books
SELECT *
FROM books;
```

#### **Explicación:**
- Al usar el asterisco (`*`), estamos seleccionando todas las columnas de la tabla `books`. Esta es una manera rápida de obtener todos los datos disponibles sin tener que escribir el nombre de cada columna.

**Resultado:** Muestra todas las columnas de la tabla **books**, que incluyen: `id`, `title`, `author`, `year`, `genre`, etc.

---

## **Lista de libros en la tabla `books`:**

| id  | title                                    | author               | year | genre         |
|-----|------------------------------------------|----------------------|------|---------------|
| 1   | 10-Day Green Smoothie Cleanse            | JJ Smith             | 2016 | Non Fiction   |
| 2   | 11/22/63: A Novel                        | Stephen King         | 2011 | Fiction       |
| 3   | 12 Rules for Life: An Antidote to Chaos  | Jordan B. Peterson   | 2018 | Non Fiction   |
| 4   | 1984 (Signet Classics)                   | George Orwell        | 2017 | Fiction       |
| 5   | 5,000 Awesome Facts (About Everything!)  | National Geographic  | 2019 | Non Fiction   |
| 6   | A Dance with Dragons                     | George R. R. Martin  | 2011 | Fiction       |
| 7   | A Game of Thrones                        | George R. R. Martin  | 2014 | Fiction       |
| 8   | A Gentleman in Moscow                    | Amor Towles          | 2017 | Fiction       |
| 9   | A Higher Loyalty                         | James Comey          | 2018 | Non Fiction   |
| 10  | A Man Called Ove                         | Fredrik Backman      | 2016 | Fiction       |

Esta tabla contiene algunos de los libros disponibles en la base de datos que estás consultando en el ejercicio.

---

## **Resumen de los conceptos clave:**

1. **SELECT**: Se utiliza para especificar las columnas que queremos obtener en los resultados. Si se usa `*`, selecciona todas las columnas.
   
2. **FROM**: Se usa para especificar la tabla de la que estamos seleccionando los datos.

3. **Comentarios en SQL**: Los comentarios, como `--`, se usan para agregar explicaciones o notas en el código que no afectan su ejecución.