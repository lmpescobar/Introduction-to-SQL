# Pregunta: Formato Correcto de Nombres en Tablas

### Descripción:
Aquí hay dos versiones de una tabla extraída de una base de datos.

¿Cuál tabla utiliza el formato de nombres correcto?

---

## Tabla 1
| ids  | customers | phone_nums   | zip_codes |
|------|-----------|--------------|-----------|
| 567  | Jelle     | 781-765-2395 | 02476     |
| 568  | Raushon   | 617-356-7772 | 01132     |
| 570  | Catalina  | 206-644-0910 | 98112     |

---

## Tabla 2
| id   | customer  | phone_num    | zip_code  |
|------|-----------|--------------|-----------|
| 567  | Jelle     | 781-765-2395 | 02476     |
| 568  | Raushon   | 617-356-7772 | 01132     |
| 570  | Catalina  | 206-644-0910 | 98112     |

---

## Posibles Respuestas:
1. **Tabla 1**
2. **Tabla 2** (Correcta)

### Respuesta correcta:
**2. Tabla 2**

---

### Explicación:
La **Tabla 2** utiliza el formato correcto de nombres según las convenciones de SQL. Los nombres de las tablas y campos deben seguir las siguientes reglas:
- **Nombres en minúsculas**: Se recomienda que los nombres de tablas y campos estén en minúsculas.
- **Nombres sin espacios**: En lugar de espacios, se utilizan guiones bajos (`_`).
- **Nombres singulares**: Los nombres de los campos suelen estar en singular, ya que cada campo representa un solo valor por registro. Por ejemplo, se usa `id`, `customer`, `phone_num`, y `zip_code`, en lugar de sus formas plurales como `ids`, `customers`, etc.

Por lo tanto, la **Tabla 2** sigue las mejores prácticas de nombrado.