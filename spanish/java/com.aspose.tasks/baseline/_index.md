---
title: "Línea base"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa los valores de línea base de un recurso."
type: docs
weight: 26
url: /es/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Representa los valores de línea base de un recurso.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | Implementación de la interfaz IComparable. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getBaselineNumber()](#getBaselineNumber--) | Obtiene el número único de un registro de datos de línea base. |
| [getBcwp()](#getBcwp--) | Obtiene el costo presupuestado de un trabajo realizado por un recurso para un proyecto hasta la fecha. |
| [getBcws()](#getBcws--) | Obtiene el costo presupuestado de un trabajo programado para un recurso. |
| [getCost()](#getCost--) | Obtiene el costo proyectado de un recurso cuando se guarda la línea base. |
| [getWork()](#getWork--) | Obtiene el trabajo asignado a un recurso cuando se guarda la línea base. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la línea base. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Devuelve un valor que indica si esta instancia es mayor que un objeto especificado. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Devuelve un valor que indica si esta instancia es menor que un objeto especificado. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Establece el número único de un registro de datos de línea base. |
| [setBcwp(double value)](#setBcwp-double-) | Establece el costo presupuestado de un trabajo realizado por un recurso para un proyecto hasta la fecha. |
| [setBcws(double value)](#setBcws-double-) | Establece el costo presupuestado de un trabajo programado para un recurso. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Establece el costo proyectado de un recurso cuando se guarda la línea base. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Establece el trabajo asignado a un recurso cuando se guarda la línea base. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | el objeto Baseline especificado con el que comparar esta instancia. |

**Returns:**
int - devuelve -1 si esta instancia es menor que el objeto especificado, 1 si esta instancia es mayor que el objeto especificado; de lo contrario devuelve 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | el objeto especificado con el que comparar esta instancia. |

**Returns:**
boolean - devuelve true si esta instancia es igual al objeto especificado; de lo contrario, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | el objeto especificado con el que comparar esta instancia. |

**Returns:**
boolean - devuelve true si esta instancia es igual al objeto especificado; de lo contrario, false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Obtiene el número único de un registro de datos de línea base.

**Returns:**
int - el número único de un registro de datos de línea base.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Obtiene el costo presupuestado de un trabajo realizado por un recurso para un proyecto hasta la fecha.

**Returns:**
double - el costo presupuestado de un trabajo realizado por un recurso para un proyecto hasta la fecha.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Obtiene el costo presupuestado de un trabajo programado para un recurso.

**Returns:**
double - el costo presupuestado de un trabajo programado para un recurso.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Obtiene el costo proyectado de un recurso cuando se guarda la línea base.

**Returns:**
java.math.BigDecimal - el costo proyectado de un recurso cuando se guarda la línea base.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Obtiene el trabajo asignado a un recurso cuando se guarda la línea base.

Valor: La cantidad de trabajo asignado a un recurso cuando se guardó la línea base.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la línea base.

**Returns:**
int - devuelve un valor de código hash para este objeto.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La primera línea base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La segunda línea base. |

**Returns:**
boolean - un valor que indica si esta instancia es igual a un objeto especificado
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Devuelve un valor que indica si esta instancia es mayor que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La primera línea base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La segunda línea base. |

**Returns:**
boolean - un valor que indica si esta instancia es mayor que un objeto especificado
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La primera línea base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La segunda línea base. |

**Returns:**
boolean - un valor que indica si esta instancia es mayor o igual que un objeto especificado
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Devuelve un valor que indica si esta instancia no es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La primera línea base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La segunda línea base. |

**Returns:**
boolean - un valor que indica si esta instancia no es igual a un objeto especificado
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Devuelve un valor que indica si esta instancia es menor que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La primera línea base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La segunda línea base. |

**Returns:**
boolean - un valor que indica si esta instancia es menor que un objeto especificado
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La primera línea base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La segunda línea base. |

**Returns:**
boolean - un valor que indica si esta instancia es menor o igual que un objeto especificado
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Establece el número único de un registro de datos de línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número único de un registro de datos de línea base. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Establece el costo presupuestado de un trabajo realizado por un recurso para un proyecto hasta la fecha.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | el costo presupuestado de un trabajo realizado por un recurso para un proyecto hasta la fecha. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Establece el costo presupuestado de un trabajo programado para un recurso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | el costo presupuestado de un trabajo programado para un recurso. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Establece el costo proyectado de un recurso cuando se guarda la línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | el costo proyectado de un recurso cuando se guarda la línea base. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Establece el trabajo asignado a un recurso cuando se guarda la línea base.

Valor: La cantidad de trabajo asignado a un recurso cuando se guardó la línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | el trabajo asignado a un recurso cuando se guarda la línea base. |

