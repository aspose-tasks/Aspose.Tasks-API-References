---
title: "Varaktighet"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar varaktighet i ett projekt."
type: docs
weight: 76
url: /sv/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Representerar varaktighet i ett projekt.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Duration()](#Duration--) | Initierar en ny instans av strukturen [Duration](../../com.aspose.tasks/duration) med ett specificerat TimeSpan‑värde och TimeUnitType. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [Clone()](#Clone--) | Skapar och returnerar en djup kopia av denna instans. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Gör en djup kopia av instansen till en annan instans. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Lägger till den specificerade varaktigheten till denna varaktighet. |
| [add(double val)](#add-double-) | Lägger till det specificerade dubbelvärdet till denna varaktighet. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Konverterar Duration‑objektet till en annan varaktighet med specificerade tidsenheter. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Returnerar ett värde som indikerar om den angivna `obj1`-instansen är lika med den angivna `obj2`-instansen. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getTimeSpan()](#getTimeSpan--) | Hämtar `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-))‑instansen för detta Duration‑objekt. |
| [getTimeUnit()](#getTimeUnit--) | Hämtar tidsenhetstypen för detta objekt. |
| [hashCode()](#hashCode--) | Returnerar ett hash‑kodvärde för detta objekt. |
| [isElapsed()](#isElapsed--) | Hämtar ett värde som indikerar om tidsenheten är förfluten. |
| [isEstimated()](#isEstimated--) | Hämtar ett värde som indikerar om tidsenheten är uppskattad. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Konverterar den specificerade strängen till en instans av strukturen [Duration](../../com.aspose.tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Tolkar varaktighetssträngen i formatet "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Subtraherar den specificerade varaktigheten från denna varaktighetsinstans. |
| [subtract(double val)](#subtract-double-) | Subtraherar det specificerade dubbelvärdet från denna varaktighetsinstans. |
| [toDouble()](#toDouble--) | Konverterar Duration‑objektet till ett `double`‑värde. |
| [toString()](#toString--) | Returnerar en strängrepresentation av denna instans. |
### Duration() {#Duration--}
```
public Duration()
```


Initierar en ny instans av strukturen [Duration](../../com.aspose.tasks/duration) med ett specificerat TimeSpan‑värde och TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Skapar och returnerar en djup kopia av denna instans.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Gör en djup kopia av instansen till en annan instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | annan instans. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Lägger till den specificerade varaktigheten till denna varaktighet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | specificerad [Duration](../../com.aspose.tasks/duration) att lägga till i denna instans. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Lägger till det specificerade dubbelvärdet till denna varaktighet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| val | double | det specificerade `double`‑värdet att lägga till i denna instans. |

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


Konverterar Duration‑objektet till en annan varaktighet med specificerade tidsenheter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| timeUnitType | byte | den specificerade tidsenhetstypen. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | Objektet att jämföra med denna instans. |

**Returns:**
boolean - Returnerar **True** om annan Duration‑instans har samma TimeSpan‑ och TimeUnit‑värden som denna instans; annars **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Returnerar ett värde som indikerar om den angivna `obj1`-instansen är lika med den angivna `obj2`-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | det första objektet att jämföra. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | det andra objektet att jämföra. |

**Returns:**
boolean - returnerar true om den specificerade `obj1`-instansen är lika med den specificerade `obj2`-instansen; annars false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet att jämföra med denna instans. |

**Returns:**
boolean - **True** om det specificerade objektet är en Duration som har samma TimeSpan‑ och TimeUnit‑värden som denna instans; annars **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Hämtar `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-))‑instansen för detta Duration‑objekt.

Värde: TimeSpan‑instansen för detta Duration‑objekt.

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) instans av detta Duration-objekt.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Hämtar tidsenhetstypen för detta objekt.

Värde: Tidsenhetstypen för denna Duration-instans.

**Returns:**
byte - tidsenhetstyp för detta objekt.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hash‑kodvärde för detta objekt.

**Returns:**
int - returnerar ett hashkodvärde för denna Duration-instans.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Hämtar ett värde som indikerar om tidsenheten är förfluten.

Värde: Flaggan som bestämmer om denna Duration-instans har förflutit.

**Returns:**
boolean - ett värde som indikerar om tidsenheten har förflutit.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Hämtar ett värde som indikerar om tidsenheten är uppskattad.

Värde: Flaggan som bestämmer om denna Duration-instans är uppskattad.

**Returns:**
boolean - ett värde som indikerar om tidsenheten är uppskattad.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Den första varaktigheten. |
| b | [Duration](../../com.aspose.tasks/duration) | Den andra varaktigheten. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är lika med ett specificerat objekt
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Den första varaktigheten. |
| b | [Duration](../../com.aspose.tasks/duration) | Den andra varaktigheten. |

**Returns:**
boolean - ett värde som indikerar om detta objekt inte är lika med ett specificerat objekt
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Konverterar den specificerade strängen till en instans av strukturen [Duration](../../com.aspose.tasks/duration).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | den angivna instansen av [Project](../../com.aspose.tasks/project) klassen för att konvertera varaktigheten för. |
| värde | java.lang.String | den angivna strängen att konvertera. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Tolkar varaktighetssträngen i formatet "PT--H--M--S--".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | den angivna strängen att tolka. |

**Returns:**
double - returnerar den analyserade instansen av `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) strukturen.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Subtraherar den specificerade varaktigheten från denna varaktighetsinstans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | den angivna [Duration](../../com.aspose.tasks/duration) instansen att subtrahera från denna instans. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Subtraherar det specificerade dubbelvärdet från denna varaktighetsinstans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| val | double | angivet `double`-värde att subtrahera från denna instans. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Konverterar Duration‑objektet till ett `double`‑värde.

**Returns:**
double - Konverterat värde.
### toString() {#toString--}
```
public String toString()
```


Returnerar en strängrepresentation av denna instans.

**Returns:**
java.lang.String - en strängrepresentation av denna instans.
