---
title: "Duration"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt de duur in een project voor."
type: docs
weight: 76
url: /nl/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Stelt de duur in een project voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Duration()](#Duration--) | Initialiseert een nieuw exemplaar van de [Duration](../../com.aspose.tasks/duration) struct met een opgegeven TimeSpan-waarde en TimeUnitType. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [Clone()](#Clone--) | Maakt en retourneert een diepe kopie van dit exemplaar. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Maakt een diepe kopie van het exemplaar naar een ander exemplaar. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Voegt de opgegeven duur toe aan deze duur. |
| [add(double val)](#add-double-) | Voegt de opgegeven double-waarde toe aan deze duur. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Converteert Duration-object naar een andere duur met opgegeven tijdseenheden. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Retourneert een waarde die aangeeft of het opgegeven `obj1`-exemplaar gelijk is aan het opgegeven `obj2`-exemplaar. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getTimeSpan()](#getTimeSpan--) | Haalt de `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\\#setTimeSpan-TimeSpan-)) instantie van dit Duration-object op. |
| [getTimeUnit()](#getTimeUnit--) | Haalt het tijdseenheidtype op voor dit object. |
| [hashCode()](#hashCode--) | Retourneert een hashcodewaarde voor dit object. |
| [isElapsed()](#isElapsed--) | Haalt een waarde op die aangeeft of de tijdseenheid verstreken is. |
| [isEstimated()](#isEstimated--) | Haalt een waarde op die aangeeft of de tijdseenheid geschat is. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Converteert de opgegeven string naar de instantie van de struct [Duration](../../com.aspose/tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Parseert de duurstring in het formaat "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Trekt de opgegeven duur af van deze duurinstantie. |
| [subtract(double val)](#subtract-double-) | Trekt de opgegeven double-waarde af van deze duurinstantie. |
| [toDouble()](#toDouble--) | Converteert Duration-object naar een `double`-waarde. |
| [toString()](#toString--) | Retourneert een tekenreeksrepresentatie van deze instantie. |
### Duration() {#Duration--}
```
public Duration()
```


Initialiseert een nieuw exemplaar van de [Duration](../../com.aspose.tasks/duration) struct met een opgegeven TimeSpan-waarde en TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Maakt en retourneert een diepe kopie van dit exemplaar.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Maakt een diepe kopie van het exemplaar naar een ander exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | een andere instantie. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Voegt de opgegeven duur toe aan deze duur.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | opgegeven [Duration](../../com.aspose/tasks/duration) om toe te voegen aan deze instantie. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Voegt de opgegeven double-waarde toe aan deze duur.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| val | double | de opgegeven `double`-waarde om toe te voegen aan deze instantie. |

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


Converteert Duration-object naar een andere duur met opgegeven tijdseenheden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| timeUnitType | byte | de opgegeven tijdseenheidtype. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | Het object om te vergelijken met deze instantie. |

**Returns:**
boolean - Retourneert **True** als een andere Duration-instantie dezelfde TimeSpan- en TimeUnit-waarden heeft als deze instantie; anders **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Retourneert een waarde die aangeeft of het opgegeven `obj1`-exemplaar gelijk is aan het opgegeven `obj2`-exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | het eerste object om te vergelijken. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | het tweede object om te vergelijken. |

**Returns:**
boolean - retourneert true als de opgegeven `obj1`-instantie gelijk is aan de opgegeven `obj2`-instantie; anders false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als het opgegeven object een Duration is die dezelfde TimeSpan- en TimeUnit-waarden heeft als deze instantie; anders **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Haalt de `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\\#setTimeSpan-TimeSpan-)) instantie van dit Duration-object op.

Waarde: De TimeSpan-instantie van dit Duration-object.

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) instantie van dit Duration-object.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Haalt het tijdseenheidtype op voor dit object.

Waarde: Het tijdseenheidtype van deze Duration-instantie.

**Returns:**
byte - tijdseenheidtype voor dit object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcodewaarde voor dit object.

**Returns:**
int - retourneert een hashcodewaarde voor deze duurinstantie.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Haalt een waarde op die aangeeft of de tijdseenheid verstreken is.

Waarde: De vlag die bepaalt of deze Duration-instantie verstreken is.

**Returns:**
boolean - een waarde die aangeeft of de tijdseenheid verstreken is.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Haalt een waarde op die aangeeft of de tijdseenheid geschat is.

Waarde: De vlag die bepaalt of deze Duration-instantie geschat is.

**Returns:**
boolean - een waarde die aangeeft of de tijdseenheid geschat is.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | De eerste duur. |
| b | [Duration](../../com.aspose.tasks/duration) | De tweede duur. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | De eerste duur. |
| b | [Duration](../../com.aspose.tasks/duration) | De tweede duur. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Converteert de opgegeven string naar de instantie van de struct [Duration](../../com.aspose/tasks/duration).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | de opgegeven instantie van de [Project](../../com.aspose.tasks/project) klasse om de duur te converteren. |
| waarde | java.lang.String | de opgegeven tekenreeks om te converteren. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Parseert de duurstring in het formaat "PT--H--M--S--".

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de opgegeven tekenreeks om te parseren. |

**Returns:**
double - retourneert een geparseerde instantie van de `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) struct.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Trekt de opgegeven duur af van deze duurinstantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | de opgegeven [Duration](../../com.aspose.tasks/duration) instantie om van deze instantie af te trekken. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Trekt de opgegeven double-waarde af van deze duurinstantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| val | double | opgegeven `double` waarde om van deze instantie af te trekken. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Converteert Duration-object naar een `double`-waarde.

**Returns:**
double - Geconverteerde waarde.
### toString() {#toString--}
```
public String toString()
```


Retourneert een tekenreeksrepresentatie van deze instantie.

**Returns:**
java.lang.String - een tekenreeksrepresentatie van deze instantie.
