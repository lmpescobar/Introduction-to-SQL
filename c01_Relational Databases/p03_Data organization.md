# Organización de Datos

## Pregunta:
Entender la organización de una base de datos es un paso importante al utilizar SQL.

### Descripción:
Observa la base de datos que se presenta a continuación. ¿Cuál de las siguientes afirmaciones describe correctamente su organización?

#### Tablas:
- **employees**: Contiene información de empleados como ID, nombre, el ID del departamento y el nivel de trabajo.
- **job_levels**: Define los niveles de trabajo y el salario mínimo correspondiente.
- **departments**: Incluye los departamentos con sus respectivos jefes.

---

### Posibles respuestas:
1. Esta es una tabla que contiene tres bases de datos relacionales: **employees**, **job_levels**, y **departments**.
2. Esta es una base de datos relacional que contiene tres tablas: **employees**, **job_levels**, y **departments**.
3. Esta es una base de datos, pero no es relacional, porque no existe relación entre los niveles de trabajo y los departamentos.
4. Esto no es una base de datos porque no se muestra código SQL.

### Respuesta correcta:
**2. Esta es una base de datos relacional que contiene tres tablas: employees, job_levels, y departments.**

---

### Explicación:
La base de datos relacional presentada contiene tres tablas: **employees**, **job_levels**, y **departments**. Las tablas en una base de datos relacional están conectadas por identificadores comunes (como **dept_id** y **job_level_id**) que permiten crear relaciones entre los datos, facilitando las consultas y el análisis.

# Tablas de la base de datos de empleados

## Tabla: employees
| id    | name    | dept_id | job_level_id |
|-------|---------|---------|--------------|
| 54378 | Darius  | 1       | 3            |
| 94722 | Raven   | 2       | 3            |
| 45783 | Eduardo | 2       | 1            |

---

## Tabla: job_levels
| id  | name        | min_salary |
|-----|-------------|------------|
| 1   | Executive   | 100000     |
| 2   | Manager     | 70000      |
| 3   | Contributor | 35000      |

---

## Tabla: departments
| id  | dept_name   | dept_head |
|-----|-------------|-----------|
| 1   | Design      | Jack      |
| 2   | Content     | Eduardo   |
| 3   | Engineering | Vanessa   |