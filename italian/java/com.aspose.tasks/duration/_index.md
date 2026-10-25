---
title: "Duration"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta la durata in un progetto."
type: docs
weight: 76
url: /it/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Rappresenta la durata in un progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Duration()](#Duration--) | Inizializza una nuova istanza della struct [Duration](../../com.aspose.tasks/duration) con un valore TimeSpan specificato e TimeUnitType. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [Clone()](#Clone--) | Crea e restituisce una copia profonda di questa istanza. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Crea una copia profonda dell'istanza in un'altra istanza. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Aggiunge la durata specificata a questa durata. |
| [add(double val)](#add-double-) | Aggiunge il valore double specificato a questa durata. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Converte l'oggetto Duration in un'altra durata con unità di tempo specificate. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Restituisce un valore che indica se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getTimeSpan()](#getTimeSpan--) | Ottiene l'istanza `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) di questo oggetto Duration. |
| [getTimeUnit()](#getTimeUnit--) | Ottiene il tipo di unità di tempo per questo oggetto. |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per questo oggetto. |
| [isElapsed()](#isElapsed--) | Ottiene un valore che indica se l'unità di tempo è trascorsa. |
| [isEstimated()](#isEstimated--) | Ottiene un valore che indica se l'unità di tempo è stimata. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Converte la stringa specificata nell'istanza della struttura [Duration](../../com.aspose.tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Analizza la stringa di durata nel formato "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Sottrae la durata specificata da questa istanza di durata. |
| [subtract(double val)](#subtract-double-) | Sottrae il valore double specificato da questa istanza di durata. |
| [toDouble()](#toDouble--) | Converte l'oggetto Duration in valore `double`. |
| [toString()](#toString--) | Restituisce una rappresentazione stringa di questa istanza. |
### Duration() {#Duration--}
```
public Duration()
```


Inizializza una nuova istanza della struct [Duration](../../com.aspose.tasks/duration) con un valore TimeSpan specificato e TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Crea e restituisce una copia profonda di questa istanza.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Crea una copia profonda dell'istanza in un'altra istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | un'altra istanza. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Aggiunge la durata specificata a questa durata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | specificato [Duration](../../com.aspose.tasks/duration) da aggiungere a questa istanza. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Aggiunge il valore double specificato a questa durata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | double | il valore `double` specificato da aggiungere a questa istanza. |

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


Converte l'oggetto Duration in un'altra durata con unità di tempo specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| timeUnitType | byte | il tipo di unità di tempo specificato. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | L'oggetto da confrontare con questa istanza. |

**Returns:**
boolean - Restituisce **True** se un'altra istanza di Duration ha gli stessi valori di TimeSpan e TimeUnit di questa istanza; altrimenti, **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Restituisce un valore che indica se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | il primo oggetto da confrontare. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | il secondo oggetto da confrontare. |

**Returns:**
boolean - restituisce true se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`; altrimenti, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto da confrontare con questa istanza. |

**Returns:**
boolean - **True** se l'oggetto specificato è un Duration che ha gli stessi valori di TimeSpan e TimeUnit di questa istanza; altrimenti, **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Ottiene l'istanza `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) di questo oggetto Duration.

Valore: L'istanza TimeSpan di questo oggetto Duration.

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) istanza di questo oggetto Duration.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Ottiene il tipo di unità di tempo per questo oggetto.

Valore: Il tipo di unità di tempo di questa istanza di Duration.

**Returns:**
byte - tipo di unità di tempo per questo oggetto.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per questo oggetto.

**Returns:**
int - restituisce un valore di codice hash per questa istanza di durata.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Ottiene un valore che indica se l'unità di tempo è trascorsa.

Valore: Il flag che determina se questa istanza di Duration è trascorsa.

**Returns:**
boolean - un valore che indica se l'unità di tempo è trascorsa.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Ottiene un valore che indica se l'unità di tempo è stimata.

Valore: Il flag che determina se questa istanza di Duration è stimata.

**Returns:**
boolean - un valore che indica se l'unità di tempo è stimata.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | La prima durata. |
| b | [Duration](../../com.aspose.tasks/duration) | La seconda durata. |

**Returns:**
boolean - un valore che indica se questa istanza è uguale a un oggetto specificato
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | La prima durata. |
| b | [Duration](../../com.aspose.tasks/duration) | La seconda durata. |

**Returns:**
boolean - un valore che indica se questa istanza non è uguale a un oggetto specificato
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Converte la stringa specificata nell'istanza della struttura [Duration](../../com.aspose.tasks/duration).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | l'istanza specificata della classe [Project](../../com.aspose.tasks/project) per convertire la durata. |
| valore | java.lang.String | la stringa specificata da convertire. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Analizza la stringa di durata nel formato "PT--H--M--S--".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la stringa specificata da analizzare. |

**Returns:**
double - restituisce l'istanza analizzata della struct `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) struct.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Sottrae la durata specificata da questa istanza di durata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | l'istanza specificata di [Duration](../../com.aspose.tasks/duration) da sottrarre da questa istanza. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Sottrae il valore double specificato da questa istanza di durata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | double | valore `double` specificato da sottrarre da questa istanza. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Converte l'oggetto Duration in valore `double`.

**Returns:**
double - Valore convertito.
### toString() {#toString--}
```
public String toString()
```


Restituisce una rappresentazione stringa di questa istanza.

**Returns:**
java.lang.String - una rappresentazione stringa di questa istanza.
