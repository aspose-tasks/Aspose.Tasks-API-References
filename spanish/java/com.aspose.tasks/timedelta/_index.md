---
title: "TimeDelta"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una diferencia entre dos marcas de tiempo."
type: docs
weight: 317
url: /es/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Representa una diferencia entre dos marcas de tiempo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Inicializa una nueva instancia de TimeDelta con el número especificado de horas, minutos y segundos. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Inicializa una nueva instancia de TimeDelta con el número especificado de días, horas, minutos, segundos y milisegundos. |
## Métodos

| Método | Descripción |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Devuelve un nuevo objeto TimeDelta cuyo valor es la suma de esta y otra instancia. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Compara dos valores TimeDelta y devuelve un entero que indica si el primer valor es más corto, igual o más largo que el segundo valor. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Compara esta instancia con un objeto TimeDelta especificado y devuelve un entero que indica si esta instancia es más corta, igual o más larga que el objeto TimeSpan. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Indica si algún intervalo de tiempo `other` es igual a este. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Comprueba dos instancias para igualdad. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Devuelve un TimeDelta que representa un número especificado de días (redondeado al milisegundo más cercano). |
| [fromHours(double value)](#fromHours-double-) | Devuelve un TimeDelta que representa un número especificado de horas (redondeado al milisegundo más cercano). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Devuelve un TimeDelta que representa un número especificado de milisegundos (redondeado al milisegundo más cercano). |
| [fromMinutes(double value)](#fromMinutes-double-) | Devuelve un TimeDelta que representa un número especificado de minutos (redondeado al milisegundo más cercano). |
| [fromSeconds(double value)](#fromSeconds-double-) | Devuelve un TimeDelta que representa un número especificado de segundos (redondeado al milisegundo más cercano). |
| [getDays()](#getDays--) | Devuelve el componente de días del intervalo de tiempo, representado por esta instancia. |
| [getHours()](#getHours--) | Devuelve el componente de horas del intervalo de tiempo, representado por esta instancia. |
| [getMilliseconds()](#getMilliseconds--) | Devuelve el componente de milisegundos del intervalo de tiempo, representado por esta instancia. |
| [getMinutes()](#getMinutes--) | Devuelve el componente de minutos del intervalo de tiempo, representado por esta instancia. |
| [getSeconds()](#getSeconds--) | Devuelve el componente de segundos del intervalo de tiempo, representado por esta instancia. |
| [getTotalDays()](#getTotalDays--) | Devuelve el valor de la instancia actual expresado en días completos y fraccionarios. |
| [getTotalHours()](#getTotalHours--) | Devuelve el valor de la instancia actual expresado en horas completas y fraccionarias. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Devuelve el valor de la instancia actual expresado en milisegundos completos y fraccionarios. |
| [getTotalMinutes()](#getTotalMinutes--) | Devuelve el valor de la instancia actual expresado en minutos completos y fraccionarios. |
| [getTotalSeconds()](#getTotalSeconds--) | Devuelve el valor de la instancia actual expresado en segundos completos y fraccionarios. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Devuelve un nuevo `TimeDelta` cuyo valor es el valor negado de esta instancia. |
| [parse(String s)](#parse-java.lang.String-) | Convierte la representación en cadena de un intervalo de tiempo a su equivalente `TimeDelta`. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Devuelve un nuevo objeto TimeDelta cuyo valor es la diferencia entre esta y las instancias `other`. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Convierte la representación en cadena de un intervalo de tiempo a su equivalente TimeDelta y devuelve un valor que indica si la conversión tuvo éxito. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Inicializa una nueva instancia de TimeDelta con el número especificado de horas, minutos y segundos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| horas | int | número de horas. |
| minutos | int | número de minutos. |
| segundos | int | número de segundos. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Inicializa una nueva instancia de TimeDelta con el número especificado de días, horas, minutos, segundos y milisegundos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| días | int | número de días. |
| horas | int | número de horas. |
| minutos | int | número de minutos. |
| segundos | int | número de segundos. |
| milisegundos | int | número de milisegundos. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Devuelve un nuevo objeto TimeDelta cuyo valor es la suma de esta y otra instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | la instancia con la que sumar. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


Compara dos valores TimeDelta y devuelve un entero que indica si el primer valor es más corto, igual o más largo que el segundo valor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | el primer intervalo de tiempo para comparar. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | el segundo intervalo de tiempo para comparar. |

**Returns:**
int - \-1 si `t1` es más corto que `t2`, 0 si `t1` es igual a `t2` y 1 si `t1` es más largo que `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Compara esta instancia con un objeto TimeDelta especificado y devuelve un entero que indica si esta instancia es más corta, igual o más larga que el objeto TimeSpan.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | una instancia para comparar. |

**Returns:**
int - \-1 si esta instancia es más corta que `other`, 0 si esta instancia es igual a `other` y 1 si esta instancia es más larga que `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Indica si algún intervalo de tiempo `other` es igual a este.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | intervalo de tiempo para comparar. |

**Returns:**
boolean - `true` si los intervalos son iguales; `false` de lo contrario.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Comprueba dos instancias para igualdad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | primera instancia. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | segunda instancia. |

**Returns:**
boolean - `true` si las instancias son iguales; `false` de lo contrario.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Devuelve un TimeDelta que representa un número especificado de días (redondeado al milisegundo más cercano).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un número de días. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Devuelve un TimeDelta que representa un número especificado de horas (redondeado al milisegundo más cercano).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un número de horas. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Devuelve un TimeDelta que representa un número especificado de milisegundos (redondeado al milisegundo más cercano).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un número de milisegundos. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Devuelve un TimeDelta que representa un número especificado de minutos (redondeado al milisegundo más cercano).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un número de minutos. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Devuelve un TimeDelta que representa un número especificado de segundos (redondeado al milisegundo más cercano).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un número de segundos. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Devuelve el componente de días del intervalo de tiempo, representado por esta instancia.

**Returns:**
int - el componente de días del intervalo de tiempo. Puede ser positivo o negativo.
### getHours() {#getHours--}
```
public int getHours()
```


Devuelve el componente de horas del intervalo de tiempo, representado por esta instancia.

**Returns:**
int - el componente de horas del intervalo de tiempo en el rango de -23 a 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Devuelve el componente de milisegundos del intervalo de tiempo, representado por esta instancia.

**Returns:**
int - el componente de milisegundos del intervalo de tiempo en el rango de -999 a 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Devuelve el componente de minutos del intervalo de tiempo, representado por esta instancia.

**Returns:**
int - el componente de minutos del intervalo de tiempo en el rango de -59 a 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Devuelve el componente de segundos del intervalo de tiempo, representado por esta instancia.

**Returns:**
int - el componente de segundos del intervalo de tiempo en el rango de -59 a 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Devuelve el valor de la instancia actual expresado en días completos y fraccionarios.

**Returns:**
double - el número total de días representado por esta instancia.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Devuelve el valor de la instancia actual expresado en horas completas y fraccionarias.

**Returns:**
double - el número total de horas representado por esta instancia.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Devuelve el valor de la instancia actual expresado en milisegundos completos y fraccionarios.

**Returns:**
double - el número total de milisegundos representado por esta instancia.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Devuelve el valor de la instancia actual expresado en minutos completos y fraccionarios.

**Returns:**
double - el número total de minutos representado por esta instancia.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Devuelve el valor de la instancia actual expresado en segundos completos y fraccionarios.

**Returns:**
double - el número total de segundos representado por esta instancia.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


Devuelve un nuevo `TimeDelta` cuyo valor es el valor negado de esta instancia.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Convierte la representación en cadena de un intervalo de tiempo a su equivalente `TimeDelta`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| s | java.lang.String | una cadena que especifica el intervalo de tiempo a convertir. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Devuelve un nuevo objeto TimeDelta cuyo valor es la diferencia entre esta y las instancias `other`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | la instancia a restar. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


Convierte la representación en cadena de un intervalo de tiempo a su equivalente TimeDelta y devuelve un valor que indica si la conversión tuvo éxito.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| s | java.lang.String | una cadena que especifica el intervalo de tiempo a convertir. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | este arreglo debe contener al menos un elemento. Cuando este método devuelve, `result[0]` contiene un objeto que representa el intervalo de tiempo especificado por `s`, o un intervalo de tiempo de longitud cero si la conversión falló. |

**Returns:**
boolean - `true` si s se convirtió correctamente; de lo contrario, `false`.
