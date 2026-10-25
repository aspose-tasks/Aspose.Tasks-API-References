---
title: "Duration"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt die Dauer in einem Projekt dar."
type: docs
weight: 76
url: /de/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Stellt die Dauer in einem Projekt dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Duration()](#Duration--) | Initialisiert eine neue Instanz der [Duration](../../com.aspose/tasks/duration) Struktur mit einem angegebenen TimeSpan-Wert und TimeUnitType. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [Clone()](#Clone--) | Erstellt und gibt eine tiefe Kopie dieser Instanz zurück. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Erstellt eine tiefe Kopie der Instanz in einer anderen Instanz. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Addiert die angegebene Dauer zu dieser Dauer. |
| [add(double val)](#add-double-) | Addiert den angegebenen double-Wert zu dieser Dauer. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Konvertiert das Duration-Objekt in eine andere Dauer mit angegebenen Zeiteinheiten. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Gibt einen Wert zurück, der angibt, ob die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getTimeSpan()](#getTimeSpan--) | Liefert die `TimeSpan`([getTimeSpan](../../com.aspose/tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose/tasks/duration\#setTimeSpan-TimeSpan-)) Instanz dieses Duration-Objekts. |
| [getTimeUnit()](#getTimeUnit--) | Liefert den Zeiteinheitstyp für dieses Objekt. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für dieses Objekt zurück. |
| [isElapsed()](#isElapsed--) | Liefert einen Wert, der angibt, ob die Zeiteinheit vergangen ist. |
| [isEstimated()](#isEstimated--) | Liefert einen Wert, der angibt, ob die Zeiteinheit geschätzt ist. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Konvertiert die angegebene Zeichenkette in die Instanz der [Duration](../../com.aspose/tasks/duration)-Struktur. |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Parst eine Dauerzeichenkette im Format "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Subtrahiert die angegebene Dauer von dieser Dauerinstanz. |
| [subtract(double val)](#subtract-double-) | Subtrahiert den angegebenen double-Wert von dieser Dauerinstanz. |
| [toDouble()](#toDouble--) | Konvertiert das Duration-Objekt in einen `double`-Wert. |
| [toString()](#toString--) | Gibt eine Zeichenkettenrepräsentation dieser Instanz zurück. |
### Duration() {#Duration--}
```
public Duration()
```


Initialisiert eine neue Instanz der [Duration](../../com.aspose/tasks/duration) Struktur mit einem angegebenen TimeSpan-Wert und TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Erstellt und gibt eine tiefe Kopie dieser Instanz zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Erstellt eine tiefe Kopie der Instanz in einer anderen Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | eine andere Instanz. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Addiert die angegebene Dauer zu dieser Dauer.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | angegebene [Duration](../../com.aspose/tasks/duration) zum Hinzufügen zu dieser Instanz. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Addiert den angegebenen double-Wert zu dieser Dauer.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| val | double | der angegebene `double` Wert, der zu dieser Instanz hinzugefügt werden soll. |

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


Konvertiert das Duration-Objekt in eine andere Dauer mit angegebenen Zeiteinheiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| timeUnitType | byte | der angegebene Zeiteinheitstyp. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | Das Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - Gibt **True** zurück, wenn die andere Duration-Instanz dieselben TimeSpan- und TimeUnit-Werte wie diese Instanz hat; andernfalls **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Gibt einen Wert zurück, der angibt, ob die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | das erste zu vergleichende Objekt. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | das zweite zu vergleichende Objekt. |

**Returns:**
boolean - gibt true zurück, wenn die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist; andernfalls false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - **True**, wenn das angegebene Objekt eine Duration ist, die dieselben TimeSpan- und TimeUnit-Werte wie diese Instanz hat; andernfalls **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Liefert die `TimeSpan`([getTimeSpan](../../com.aspose/tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose/tasks/duration\#setTimeSpan-TimeSpan-)) Instanz dieses Duration-Objekts.

Wert: Die TimeSpan-Instanz dieses Duration-Objekts.

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-))-Instanz dieses Duration-Objekts.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Liefert den Zeiteinheitstyp für dieses Objekt.

Wert: Der Zeiteinheitstyp dieser Duration-Instanz.

**Returns:**
byte - Zeiteinheitstyp für dieses Objekt.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für dieses Objekt zurück.

**Returns:**
int - gibt einen Hash-Code-Wert für diese Duration-Instanz zurück.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Liefert einen Wert, der angibt, ob die Zeiteinheit vergangen ist.

Wert: Das Flag, das bestimmt, ob diese Duration-Instanz abgelaufen ist.

**Returns:**
boolean - ein Wert, der angibt, ob die Zeiteinheit abgelaufen ist.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Liefert einen Wert, der angibt, ob die Zeiteinheit geschätzt ist.

Wert: Das Flag, das bestimmt, ob diese Duration-Instanz geschätzt ist.

**Returns:**
boolean - ein Wert, der angibt, ob die Zeiteinheit geschätzt ist.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Die erste Dauer. |
| b | [Duration](../../com.aspose.tasks/duration) | Die zweite Dauer. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Die erste Dauer. |
| b | [Duration](../../com.aspose.tasks/duration) | Die zweite Dauer. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Konvertiert die angegebene Zeichenkette in die Instanz der [Duration](../../com.aspose/tasks/duration)-Struktur.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | die angegebene Instanz der Klasse [Project](../../com.aspose.tasks/project), für die die Dauer konvertiert werden soll. |
| Wert | java.lang.String | die angegebene Zeichenkette zum Konvertieren. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Parst eine Dauerzeichenkette im Format "PT--H--M--S--".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die angegebene Zeichenkette zum Parsen. |

**Returns:**
double - gibt die geparste Instanz der `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-))-Struktur zurück.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Subtrahiert die angegebene Dauer von dieser Dauerinstanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | die angegebene [Duration](../../com.aspose.tasks/duration)-Instanz, die von dieser Instanz subtrahiert werden soll. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Subtrahiert den angegebenen double-Wert von dieser Dauerinstanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| val | double | angegebener `double`-Wert, der von dieser Instanz subtrahiert werden soll. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Konvertiert das Duration-Objekt in einen `double`-Wert.

**Returns:**
double - konvertierter Wert.
### toString() {#toString--}
```
public String toString()
```


Gibt eine Zeichenkettenrepräsentation dieser Instanz zurück.

**Returns:**
java.lang.String - eine Zeichenkettenrepräsentation dieser Instanz.
