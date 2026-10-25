---
title: "Duration"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa la duración en un proyecto."
type: docs
weight: 76
url: /es/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Representa la duración en un proyecto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Duration()](#Duration--) | Inicializa una nueva instancia de la estructura [Duration](../../com.aspose.tasks/duration) con un valor de TimeSpan especificado y TimeUnitType. |
## Métodos

| Método | Descripción |
| --- | --- |
| [Clone()](#Clone--) | Crea y devuelve una copia profunda de esta instancia. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Realiza una copia profunda de la instancia en otra instancia. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Añade la duración especificada a esta duración. |
| [add(double val)](#add-double-) | Añade el valor double especificado a esta duración. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Convierte el objeto Duration a otra duración con unidades de tiempo especificadas. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Devuelve un valor que indica si la instancia `obj1` especificada es igual a la instancia `obj2` especificada. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getTimeSpan()](#getTimeSpan--) | Obtiene la instancia `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) de este objeto Duration. |
| [getTimeUnit()](#getTimeUnit--) | Obtiene el tipo de unidad de tiempo para este objeto. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para este objeto. |
| [isElapsed()](#isElapsed--) | Obtiene un valor que indica si la unidad de tiempo está transcurrida. |
| [isEstimated()](#isEstimated--) | Obtiene un valor que indica si la unidad de tiempo es estimada. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Convierte la cadena especificada a la instancia de la estructura [Duration](../../com.aspose.tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Analiza la cadena de duración en el formato "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Resta la duración especificada de esta instancia de duración. |
| [subtract(double val)](#subtract-double-) | Resta el valor double especificado de esta instancia de duración. |
| [toDouble()](#toDouble--) | Convierte el objeto Duration a un valor `double`. |
| [toString()](#toString--) | Devuelve una representación en cadena de esta instancia. |
### Duration() {#Duration--}
```
public Duration()
```


Inicializa una nueva instancia de la estructura [Duration](../../com.aspose.tasks/duration) con un valor de TimeSpan especificado y TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Crea y devuelve una copia profunda de esta instancia.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Realiza una copia profunda de la instancia en otra instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | otra instancia. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Añade la duración especificada a esta duración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | [Duration](../../com.aspose.tasks/duration) especificado para agregar a esta instancia. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Añade el valor double especificado a esta duración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| val | double | el valor `double` especificado para agregar a esta instancia. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Convierte el objeto Duration a otra duración con unidades de tiempo especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| timeUnitType | byte | el tipo de unidad de tiempo especificado. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | El objeto para comparar con esta instancia. |

**Returns:**
boolean - Devuelve **True** si otra instancia de Duration tiene los mismos valores de TimeSpan y TimeUnit que esta instancia; de lo contrario, **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Devuelve un valor que indica si la instancia `obj1` especificada es igual a la instancia `obj2` especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | el primer objeto a comparar. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | el segundo objeto a comparar. |

**Returns:**
boolean - devuelve true si la instancia especificada `obj1` es igual a la instancia especificada `obj2`; de lo contrario, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto para comparar con esta instancia. |

**Returns:**
boolean - **True** si el objeto especificado es un Duration que tiene los mismos valores de TimeSpan y TimeUnit que esta instancia; de lo contrario, **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Obtiene la instancia `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) de este objeto Duration.

Valor: La instancia de TimeSpan de este objeto Duration.

**Returns:**
double - instancia de `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) de este objeto Duration.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Obtiene el tipo de unidad de tiempo para este objeto.

Valor: El tipo de unidad de tiempo de esta instancia de Duration.

**Returns:**
byte - tipo de unidad de tiempo para este objeto.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para este objeto.

**Returns:**
int - devuelve un valor de código hash para esta instancia de duración.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Obtiene un valor que indica si la unidad de tiempo está transcurrida.

Valor: La bandera que determina si esta instancia de Duration está transcurrida.

**Returns:**
boolean - un valor que indica si la unidad de tiempo está transcurrida.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Obtiene un valor que indica si la unidad de tiempo es estimada.

Valor: La bandera que determina si esta instancia de Duration es estimada.

**Returns:**
boolean - un valor que indica si la unidad de tiempo es estimada.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | La primera duración. |
| b | [Duration](../../com.aspose.tasks/duration) | La segunda duración. |

**Returns:**
boolean - un valor que indica si esta instancia es igual a un objeto especificado
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Devuelve un valor que indica si esta instancia no es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | La primera duración. |
| b | [Duration](../../com.aspose.tasks/duration) | La segunda duración. |

**Returns:**
boolean - un valor que indica si esta instancia no es igual a un objeto especificado
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Convierte la cadena especificada a la instancia de la estructura [Duration](../../com.aspose.tasks/duration).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | la instancia especificada de la clase [Project](../../com.aspose.tasks/project) para convertir la duración. |
| valor | java.lang.String | la cadena especificada para convertir. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Analiza la cadena de duración en el formato "PT--H--M--S--".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la cadena especificada para analizar. |

**Returns:**
double - devuelve la instancia analizada del struct `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)).
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Resta la duración especificada de esta instancia de duración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | la instancia especificada de [Duration](../../com.aspose.tasks/duration) para restar de esta instancia. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Resta el valor double especificado de esta instancia de duración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| val | double | valor `double` especificado para restar de esta instancia. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Convierte el objeto Duration a un valor `double`.

**Returns:**
double - Valor convertido.
### toString() {#toString--}
```
public String toString()
```


Devuelve una representación en cadena de esta instancia.

**Returns:**
java.lang.String - una representación en cadena de esta instancia.
