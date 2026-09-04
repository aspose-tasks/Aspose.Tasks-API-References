---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Differenz zwischen zwei Zeitstempeln dar."
type: docs
weight: 317
url: /de/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Stellt eine Differenz zwischen zwei Zeitstempeln dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Initialisiert eine neue Instanz von TimeDelta mit der angegebenen Anzahl von Stunden, Minuten und Sekunden. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Initialisiert eine neue Instanz von TimeDelta mit der angegebenen Anzahl von Tagen, Stunden, Minuten, Sekunden und Millisekunden. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Gibt ein neues TimeDelta-Objekt zurück, dessen Wert die Summe dieser und einer anderen Instanz ist. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Vergleicht zwei TimeDelta-Werte und gibt einen Integer zurück, der angibt, ob der erste Wert kürzer, gleich oder länger als der zweite Wert ist. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Vergleicht diese Instanz mit einem angegebenen TimeDelta-Objekt und gibt einen Integer zurück, der angibt, ob diese Instanz kürzer, gleich oder länger als das TimeSpan-Objekt ist. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Gibt an, ob ein `other`-Zeitintervall diesem entspricht. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Überprüft zwei Instanzen auf Gleichheit. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Tagen darstellt (auf die nächste Millisekunde gerundet). |
| [fromHours(double value)](#fromHours-double-) | Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Stunden darstellt (auf die nächste Millisekunde gerundet). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Millisekunden darstellt (auf die nächste Millisekunde gerundet). |
| [fromMinutes(double value)](#fromMinutes-double-) | Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Minuten darstellt (auf die nächste Millisekunde gerundet). |
| [fromSeconds(double value)](#fromSeconds-double-) | Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Sekunden darstellt (auf die nächste Millisekunde gerundet). |
| [getDays()](#getDays--) | Gibt die Tageskomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird. |
| [getHours()](#getHours--) | Gibt die Stundenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird. |
| [getMilliseconds()](#getMilliseconds--) | Gibt die Millisekundenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird. |
| [getMinutes()](#getMinutes--) | Gibt die Minutenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird. |
| [getSeconds()](#getSeconds--) | Gibt die Sekundenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird. |
| [getTotalDays()](#getTotalDays--) | Gibt den Wert der aktuellen Instanz in ganzen und Bruchteilen von Tagen zurück. |
| [getTotalHours()](#getTotalHours--) | Gibt den Wert der aktuellen Instanz in ganzen und Bruchteilen von Stunden zurück. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Gibt den Wert der aktuellen Instanz in ganzen und Bruchteilen von Millisekunden zurück. |
| [getTotalMinutes()](#getTotalMinutes--) | Gibt den Wert der aktuellen Instanz zurück, ausgedrückt in ganzen und Bruchteilen von Minuten. |
| [getTotalSeconds()](#getTotalSeconds--) | Gibt den Wert der aktuellen Instanz zurück, ausgedrückt in ganzen und Bruchteilen von Sekunden. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Gibt ein neues `TimeDelta` zurück, dessen Wert der negierte Wert dieser Instanz ist. |
| [parse(String s)](#parse-java.lang.String-) | Konvertiert die Zeichenkettenrepräsentation eines Zeitintervalls in das entsprechende `TimeDelta`. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Gibt ein neues TimeDelta-Objekt zurück, dessen Wert die Differenz zwischen dieser und `other` Instanzen ist. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Konvertiert die Zeichenkettenrepräsentation eines Zeitintervalls in das entsprechende TimeDelta und gibt einen Wert zurück, der angibt, ob die Konvertierung erfolgreich war. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Initialisiert eine neue Instanz von TimeDelta mit der angegebenen Anzahl von Stunden, Minuten und Sekunden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stunden | int | Anzahl der Stunden. |
| Minuten | int | Anzahl der Minuten. |
| Sekunden | int | Anzahl der Sekunden. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Initialisiert eine neue Instanz von TimeDelta mit der angegebenen Anzahl von Tagen, Stunden, Minuten, Sekunden und Millisekunden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Tage | int | Anzahl der Tage. |
| Stunden | int | Anzahl der Stunden. |
| Minuten | int | Anzahl der Minuten. |
| Sekunden | int | Anzahl der Sekunden. |
| Millisekunden | int | Anzahl der Millisekunden. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Gibt ein neues TimeDelta-Objekt zurück, dessen Wert die Summe dieser und einer anderen Instanz ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | die Instanz, mit der summiert werden soll. |

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


Vergleicht zwei TimeDelta-Werte und gibt einen Integer zurück, der angibt, ob der erste Wert kürzer, gleich oder länger als der zweite Wert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | das erste Zeitintervall zum Vergleichen. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | das zweite Zeitintervall zum Vergleichen. |

**Returns:**
int - \-1 wenn `t1` kürzer ist als `t2`, 0 wenn `t1` gleich `t2` ist und 1 wenn `t1` länger ist als `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Vergleicht diese Instanz mit einem angegebenen TimeDelta-Objekt und gibt einen Integer zurück, der angibt, ob diese Instanz kürzer, gleich oder länger als das TimeSpan-Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | eine Instanz zum Vergleichen. |

**Returns:**
int - \-1 wenn diese Instanz kürzer ist als `other`, 0 wenn diese Instanz gleich `other` ist und 1 wenn diese Instanz länger ist als `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Gibt an, ob ein `other`-Zeitintervall diesem entspricht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | Zeitspanne zum Vergleichen. |

**Returns:**
boolean - `true` wenn Intervalle gleich sind; `false` sonst.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Überprüft zwei Instanzen auf Gleichheit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | erste Instanz. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | zweite Instanz. |

**Returns:**
boolean - `true`, wenn Instanzen gleich sind; `false` sonst.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| andere | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Tagen darstellt (auf die nächste Millisekunde gerundet).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | eine Anzahl von Tagen. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Stunden darstellt (auf die nächste Millisekunde gerundet).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | eine Anzahl von Stunden. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Millisekunden darstellt (auf die nächste Millisekunde gerundet).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | eine Anzahl von Millisekunden. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Minuten darstellt (auf die nächste Millisekunde gerundet).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | eine Anzahl von Minuten. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Gibt ein TimeDelta zurück, das eine angegebene Anzahl von Sekunden darstellt (auf die nächste Millisekunde gerundet).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | eine Anzahl von Sekunden. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Gibt die Tageskomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird.

**Returns:**
int - die Tageskomponente des Zeitintervalls. Kann positiv oder negativ sein.
### getHours() {#getHours--}
```
public int getHours()
```


Gibt die Stundenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird.

**Returns:**
int - die Stundenkomponente des Zeitintervalls im Bereich von -23 bis 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Gibt die Millisekundenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird.

**Returns:**
int - die Millisekundenkomponente des Zeitintervalls im Bereich von -999 bis 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Gibt die Minutenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird.

**Returns:**
int - die Minutenkomponente des Zeitintervalls im Bereich von -59 bis 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Gibt die Sekundenkomponente des Zeitintervalls zurück, das von dieser Instanz dargestellt wird.

**Returns:**
int - die Sekundenkomponente des Zeitintervalls im Bereich von -59 bis 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Gibt den Wert der aktuellen Instanz in ganzen und Bruchteilen von Tagen zurück.

**Returns:**
double - die Gesamtanzahl der Tage, die durch diese Instanz dargestellt werden.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Gibt den Wert der aktuellen Instanz in ganzen und Bruchteilen von Stunden zurück.

**Returns:**
double - die Gesamtanzahl der Stunden, die durch diese Instanz dargestellt werden.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Gibt den Wert der aktuellen Instanz in ganzen und Bruchteilen von Millisekunden zurück.

**Returns:**
double - die Gesamtanzahl der Millisekunden, die durch diese Instanz dargestellt werden.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Gibt den Wert der aktuellen Instanz zurück, ausgedrückt in ganzen und Bruchteilen von Minuten.

**Returns:**
double - die Gesamtanzahl der Minuten, die durch diese Instanz dargestellt werden.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Gibt den Wert der aktuellen Instanz zurück, ausgedrückt in ganzen und Bruchteilen von Sekunden.

**Returns:**
double - die Gesamtanzahl der Sekunden, die durch diese Instanz dargestellt werden.
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


Gibt ein neues `TimeDelta` zurück, dessen Wert der negierte Wert dieser Instanz ist.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Konvertiert die Zeichenkettenrepräsentation eines Zeitintervalls in das entsprechende `TimeDelta`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | java.lang.String | ein String, der das zu konvertierende Zeitintervall angibt. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Gibt ein neues TimeDelta-Objekt zurück, dessen Wert die Differenz zwischen dieser und `other` Instanzen ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | die zu subtrahierende Instanz. |

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


Konvertiert die Zeichenkettenrepräsentation eines Zeitintervalls in das entsprechende TimeDelta und gibt einen Wert zurück, der angibt, ob die Konvertierung erfolgreich war.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | java.lang.String | ein String, der das zu konvertierende Zeitintervall angibt. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | Dieses Array muss mindestens ein Element enthalten. Wenn diese Methode zurückkehrt, enthält `result[0]` ein Objekt, das das durch `s` angegebene Zeitintervall darstellt, oder ein Zeitintervall mit Länge null, falls die Konvertierung fehlgeschlagen ist. |

**Returns:**
boolean - `true`, wenn s erfolgreich konvertiert wurde; sonst `false`.
