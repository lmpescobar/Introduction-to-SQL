# Ejercicio: Explorando la Tabla `books` - Explicación de `SELECT` y `FROM`

---

## Descripción:
En este ejercicio, ejecutamos una consulta SQL para explorar la tabla **books**. La consulta SQL utilizada es:

```sql
SELECT *
FROM books;
```

---

## Explicación de la Consulta:

### 1. `SELECT`
La palabra clave **`SELECT`** se utiliza para especificar qué columnas de la base de datos queremos ver en el resultado de nuestra consulta.

- **`*`**: El asterisco (`*`) es un comodín que indica que queremos seleccionar **todas** las columnas de la tabla. En este caso, seleccionamos todas las columnas de la tabla **books** (como `id`, `title`, `author`, `year`, `genre`).
  
  Si en lugar de `*` hubiéramos puesto, por ejemplo, `title, author`, solo se mostrarían las columnas **title** y **author**.

### 2. `FROM`
La palabra clave **`FROM`** se utiliza para especificar **de qué tabla** queremos obtener los datos.

- **`books`**: Aquí estamos indicando que los datos deben ser extraídos de la tabla llamada **books**. Esta tabla contiene información relacionada con libros, como el título, el autor, el año de publicación, y el género.

### Función Combinada:
La consulta completa:

```sql
SELECT *
FROM books;
```

- **`SELECT *`** indica que queremos ver todas las columnas de la tabla.
- **`FROM books`** especifica que los datos deben venir de la tabla llamada **books**.

---

## Resultado de la Consulta:

La consulta devuelve todas las filas y columnas de la tabla **books**. Aquí tienes un ejemplo de algunas filas:

| id  | title                                         | author                   | year | genre         |
|-----|-----------------------------------------------|--------------------------|------|---------------|
| 1   | 10-Day Green Smoothie Cleanse                 | JJ Smith                  | 2016 | Non Fiction   |
| 2   | 11/22/63: A Novel                             | Stephen King              | 2011 | Fiction       |
| 3   | 12 Rules for Life: An Antidote to Chaos       | Jordan B. Peterson        | 2018 | Non Fiction   |
| 4   | 1984 (Signet Classics)                        | George Orwell             | 2017 | Fiction       |
| 5   | 5,000 Awesome Facts (National Geographic Kids)| National Geographic Kids  | 2019 | Non Fiction   |
| 6   | A Dance with Dragons (A Song of Ice and Fire) | George R. R. Martin       | 2011 | Fiction       |

---

## Resumen:
- **`SELECT`** nos permite elegir las columnas que queremos ver. Si usamos `*`, estamos seleccionando todas las columnas.
- **`FROM`** nos indica de qué tabla provienen los datos. En este caso, de la tabla **books**.

Este es el fundamento básico de las consultas en SQL, y es muy útil para explorar o extraer información de tablas de bases de datos.