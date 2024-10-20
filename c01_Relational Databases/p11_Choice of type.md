# Ejercicio: Elección de Tipo de Dato

### Descripción:
Al crear una tabla en una base de datos, es crucial seleccionar el **tipo de dato adecuado** para cada campo. Los tipos de datos permiten que la base de datos almacene la información de manera eficiente y aseguran que las operaciones que se realicen sobre esos datos sean válidas. Cada campo en una tabla debe tener un tipo de dato asociado que defina cómo los valores serán almacenados y manipulados.

Este ejercicio te ayudará a entender cómo elegir el tipo de dato correcto para diferentes tipos de información.

---

## Instrucciones:
- Organiza cada elemento en el tipo de dato más adecuado para su almacenamiento.

---

## Opciones:

### 1. **VARCHAR** (Variable Character):
Este tipo de dato se utiliza para almacenar **cadenas de texto de longitud variable**. Es ideal para campos donde la longitud del texto puede variar de un registro a otro, como nombres, descripciones, direcciones o comentarios.

#### Ejemplos de uso:
- **Comentarios de productos escritos por clientes**: Cada cliente puede dejar una reseña diferente en longitud, por lo que el campo debe poder ajustarse a la longitud variable de cada comentario.
- **Números de teléfono**: Aunque contienen números, los números de teléfono no son utilizados para cálculos matemáticos, y suelen tener guiones o paréntesis, lo cual los convierte en cadenas de texto, no en números.

#### Características:
- Flexible en cuanto a la longitud del texto.
- Almacena solo el espacio que necesita para el texto (no predefine un espacio fijo).
  
---

### 2. **INT** (Integer - Entero):
El tipo **INT** se utiliza para almacenar **números enteros**, es decir, números sin decimales. Los enteros son útiles cuando necesitas almacenar datos numéricos que representen cantidades enteras, como años, contadores, identificadores o cantidades.

#### Ejemplos de uso:
- **Año del modelo**: Un año como "2004" es un número entero que no tiene parte decimal, por lo que se almacena de manera eficiente como un **INT**.
- **Número de suscriptores de la lista de correos**: El número de suscriptores es un conteo entero (sin fracciones), lo que lo convierte en un dato ideal para ser almacenado como **INT**.

#### Características:
- Puede almacenar números desde -2,147,483,648 hasta 2,147,483,647 (en SQL estándar).
- Adecuado para datos que no requieren precisión decimal.

---

### 3. **NUMERIC** (Números decimales o de punto flotante):
El tipo de dato **NUMERIC** se utiliza para almacenar **números que incluyen fracciones o decimales**. Es crucial cuando se requiere precisión en los cálculos, como en precios, pesos o porcentajes.

#### Ejemplos de uso:
- **Precios de productos**: Los precios como "63.75" tienen una parte decimal que es importante para garantizar la precisión en cálculos financieros. Almacenar los precios como **NUMERIC** asegura que se pueda calcular con exactitud.
- **Peso en toneladas**: Los pesos, como "5.67", necesitan parte decimal para representar correctamente el valor, especialmente en contextos donde la precisión es clave (por ejemplo, en la logística o el transporte).

#### Características:
- Mantiene precisión exacta, lo cual es fundamental para operaciones financieras o cálculos científicos.
- Puede definir cuántos dígitos se permiten antes y después del punto decimal (por ejemplo, `NUMERIC(10, 2)` permitiría 10 dígitos en total, 2 de ellos después del punto decimal).

---

## Resumen de Tipos de Datos:

- **VARCHAR** es ideal para texto o datos que contienen caracteres alfabéticos y numéricos que no se usan para cálculos (como nombres o números de teléfono).
- **INT** es el tipo de dato adecuado para almacenar cantidades enteras que no requieren decimales (como años o cantidades).
- **NUMERIC** es necesario cuando los datos tienen una parte decimal y la precisión es importante, como en los precios o medidas.

### Consideraciones adicionales:
1. **Eficiencia en el almacenamiento**: Elegir el tipo de dato correcto ayuda a optimizar el almacenamiento de la base de datos. Por ejemplo, usar **VARCHAR** para números no es eficiente si esos números se van a usar para cálculos.
2. **Operaciones válidas**: Algunos tipos de operaciones solo son válidos para ciertos tipos de datos. Por ejemplo, las operaciones matemáticas como la suma o la multiplicación solo se pueden realizar sobre tipos de datos numéricos, como **INT** o **NUMERIC**, no sobre cadenas de texto.
3. **Precisión**: Los tipos de datos como **NUMERIC** aseguran precisión en los cálculos, lo cual es esencial para campos que requieren un alto grado de exactitud, como los precios.

---