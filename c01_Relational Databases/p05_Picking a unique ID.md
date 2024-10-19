# Pregunta: Seleccionando un ID único

### Descripción:
Un **identificador único** es un valor que distingue un registro de otros en la misma tabla.

En la tabla **employees**, ¿qué campo crees que es la opción más adecuada como identificador único?

---

## Tabla: employees
| id    | name    | dept_id | job_level_id |
|-------|---------|---------|--------------|
| 54378 | Darius  | 1       | 3            |
| 94722 | Raven   | 2       | 3            |
| 45783 | Eduardo | 2       | 1            |

---

## Posibles respuestas:
1. **name**
2. **dept_id**
3. **year_hired**
4. **id** (Correcta)

### Respuesta correcta:
**4. id**

---

### Explicación:
El campo **id** es la mejor opción para un identificador único porque asigna un valor único a cada registro en la tabla. Este valor es irrepetible, lo que garantiza que cada empleado sea identificado de manera única. Otras columnas como **name** podrían tener valores duplicados, como el caso de dos empleados con el mismo nombre, y por lo tanto no serían buenos identificadores únicos.