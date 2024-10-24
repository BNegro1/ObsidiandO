## JOINS y SQL

### Tipos de JOINS

#### JOINS
La unión de tablas en SQL permite combinar datos de múltiples fuentes en una consulta. Existen diversos tipos de JOINS para adaptarse a diferentes necesidades.

### Calificación y optimización de consultas
Cuando se unen tablas en SQL, es crucial calificar los nombres de las columnas para evitar ambigüedades y optimizar el rendimiento.

### Cláusulas

#### Cláusula USING
La cláusula **USING** facilita JOINS cuando hay columnas con nombres idénticos en las tablas. Permite especificar qué columnas deben utilizarse para la unión de igualdad.

Ejemplo de **INNER JOIN** con Cláusula **USING**:

```sql
SELECT columna1, columna2
FROM tabla1
INNER JOIN tabla2 **USING** (columna);
```

Ejemplo de **LEFT JOIN** con Cláusula **USING**:

```sql
SELECT columna1, columna2
FROM tabla1
LEFT JOIN tabla2 **USING** (columna);
```

Ejemplo de **RIGHT JOIN** con Cláusula **USING**:

```sql
SELECT columna1, columna2
FROM tabla1
RIGHT JOIN tabla2 **USING** (columna);
```

Ejemplo de **FULL JOIN** con Cláusula **USING**:

```sql
SELECT columna1, columna2
FROM tabla1
FULL JOIN tabla2 **USING** (columna);
```

Ejemplo de **CROSS JOIN** con Cláusula **USING**:

```sql
SELECT columna1, columna2
FROM tabla1
CROSS JOIN tabla2;
```

#### Cláusula ON
La cláusula **ON** se emplea para crear JOINS especificando las columnas de unión entre dos tablas, permitiendo flexibilidad en casos de columnas con nombres diferentes.

Ejemplo de **INNER JOIN** con Cláusula **ON**:

```sql
SELECT columna1, columna2
FROM tabla1
INNER JOIN tabla2 **ON** tabla1.columna = tabla2.columna;
```

Ejemplo de **LEFT JOIN** con Cláusula **ON**:

```sql
SELECT columna1, columna2
FROM tabla1
LEFT JOIN tabla2 **ON** tabla1.columna = tabla2.columna;
```

Ejemplo de **RIGHT JOIN** con Cláusula **ON**:

```sql
SELECT columna1, columna2
FROM tabla1
RIGHT JOIN tabla2 **ON** tabla1.columna = tabla2.columna;
```

Ejemplo de **FULL JOIN** con Cláusula **ON**:

```sql
SELECT columna1, columna2
FROM tabla1
FULL JOIN tabla2 **ON** tabla1.columna = tabla2.columna;
```

Ejemplo de **CROSS JOIN** con Cláusula **ON**:

```sql
SELECT columna1, columna2
FROM tabla1
CROSS JOIN tabla2;
```

#### Agregando Condiciones Adicionales a un Join
Para agregar una condición a la cláusula **USING**, se debe usar la cláusula **WHERE**. Si se desea incorporar más condiciones, se deben agregar las cláusulas **AND** y **OR** que se requieran a continuación de la cláusula **WHERE**.

Para agregar una condición a la cláusula **ON**, se puede usar la cláusula de condición **WHERE** o el operador lógico **AND**. Si se desea incorporar más condiciones, se deben agregar las cláusulas **AND** y **OR** que se deseen.

Ejemplo de Agregando Condiciones Adicionales a un Join:

```sql
SELECT columna1, columna2
FROM tabla1
INNER JOIN tabla2 ON tabla1.columna = tabla2.columna
WHERE tabla1.otra_columna = 'valor' AND tabla2.columna3 > 100;
```