## Masterclass: Sabores de SQL

### Introducción

En el mundo de las bases de datos relacionales, **SQL** es el lenguaje estándar para interactuar con los datos. Sin embargo, existen diferentes "sabores" o versiones de SQL que se utilizan en diferentes sistemas de bases de datos. Aunque la mayoría de las palabras clave son compartidas entre estos sabores, algunas diferencias y características adicionales los distinguen entre sí. En esta masterclass exploraremos algunos de los sabores más populares de SQL, cómo se comparan y por qué no deberías preocuparte demasiado por elegir uno específico para comenzar.

---

### ¿Qué es un sabor de SQL?

SQL, al ser un estándar para las bases de datos relacionales, tiene diferentes **sabores** o variantes, cada uno desarrollado para ser utilizado con un sistema específico de gestión de bases de datos. Algunos sabores son **gratuitos** y de **código abierto**, mientras que otros son de **pago** y cuentan con soporte técnico. 

Lo importante es que **todos los sabores de SQL deben seguir los estándares universales** establecidos por la **Organización Internacional de Normas** (ISO) y el **Instituto Nacional Estadounidense de Estándares** (ANSI). Esto significa que, en su mayoría, comparten las mismas palabras clave y funcionalidades básicas. Las diferencias entre ellos suelen residir en **funcionalidades adicionales** o características específicas de un sistema particular.

---

### Dos sabores populares de SQL

Entre los sabores de SQL más conocidos están **PostgreSQL** y **SQL Server**:

- **PostgreSQL**: Este sistema de bases de datos relacional es **gratuito** y de **código abierto**. Fue desarrollado originalmente en la Universidad de California, Berkeley, con el patrocinio de la famosa **Defense Advanced Research Projects Agency (DARPA)**. Además, es conocido por su robustez y escalabilidad, siendo ampliamente utilizado en proyectos que requieren sistemas de bases de datos avanzados. PostgreSQL es tanto el nombre del sistema de bases de datos como del sabor SQL que se utiliza con él.

- **SQL Server**: Desarrollado por **Microsoft**, este sistema de bases de datos también es relacional y tiene tanto versiones gratuitas como empresariales. Su sabor de SQL se llama **T-SQL** y está diseñado para integrarse perfectamente con otros productos de Microsoft, lo que lo convierte en una opción popular para empresas que ya están inmersas en el ecosistema de Microsoft.

---

### Comparando PostgreSQL y SQL Server

Un buen modo de entender los sabores de SQL es pensar en ellos como **dialectos del mismo idioma**. Por ejemplo, una persona que habla inglés estadounidense entenderá a alguien que hable inglés británico, aunque haya algunas diferencias menores entre ambos.

En SQL, un ejemplo de estas diferencias es cómo se limita el número de registros devueltos por una consulta. En **PostgreSQL**, usamos la palabra clave **LIMIT** para limitar el número de registros. Sin embargo, en **SQL Server**, la palabra clave equivalente es **TOP**. A pesar de esta diferencia en palabras clave, el resultado es exactamente el mismo en ambos casos.

**Ejemplo de código**:

En **PostgreSQL**:
```sql
SELECT name, id
FROM employees
LIMIT 2;
```

En **SQL Server**:
```sql
SELECT TOP 2 name, id
FROM employees;
```

Este tipo de diferencias es pequeño y no afecta significativamente la capacidad de aprender o trabajar con un sabor de SQL u otro. 

---

### ¿Qué sabor de SQL deberías aprender?

Para los nuevos aprendices de SQL, puede ser tentador preguntarse **qué sabor de SQL aprender primero**. Si trabajas en una empresa que utiliza SQL Server, entonces tiene sentido que aprendas **T-SQL**. Si estás buscando un enfoque más amplio y flexible, **PostgreSQL** puede ser una buena opción, ya que es de código abierto y ampliamente utilizado.

Lo bueno es que las diferencias entre los sabores de SQL son mínimas. Si aprendes uno, cambiarte a otro será relativamente sencillo, ya que comparten más similitudes que diferencias. **Un experto en PostgreSQL puede convertirse en un experto en SQL Server** con solo aprender algunas palabras clave adicionales y ligeros cambios en la sintaxis.

---

### Conclusión

En resumen, los sabores de SQL como PostgreSQL y SQL Server comparten muchas características y palabras clave. Las diferencias entre ellos son menores, y aprender uno te permitirá adaptarte rápidamente a otros sabores. Elige el que mejor se adapte a tus necesidades actuales, pero no te preocupes demasiado por la elección, ya que dominar un sabor te facilitará aprender los demás.

---

### ¡A Practicar!

Con todo este conocimiento sobre los sabores de SQL, es hora de practicar con algunas consultas en los diferentes dialectos. ¡Vamos allá!