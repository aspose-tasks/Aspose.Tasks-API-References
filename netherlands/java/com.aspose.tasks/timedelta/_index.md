---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een verschil tussen twee tijdstempels voor."
type: docs
weight: 317
url: /nl/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Stelt een verschil tussen twee tijdstempels voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Initialiseert een nieuwe instantie van TimeDelta met het opgegeven aantal uren, minuten en seconden. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Initialiseert een nieuwe instantie van TimeDelta met het opgegeven aantal dagen, uren, minuten, seconden en milliseconden. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Retourneert een nieuw TimeDelta-object waarvan de waarde de som is van deze en een andere instantie. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Vergelijkt twee TimeDelta-waarden en retourneert een geheel getal dat aangeeft of de eerste waarde korter, gelijk aan of langer is dan de tweede waarde. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Vergelijkt deze instantie met een opgegeven TimeDelta-object en retourneert een geheel getal dat aangeeft of deze instantie korter, gelijk aan of langer is dan het TimeSpan-object. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Geeft aan of een bepaalde `other` tijdsduur gelijk is aan deze. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Controleert twee instanties op gelijkheid. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Retourneert een TimeDelta die een opgegeven aantal dagen vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde). |
| [fromHours(double value)](#fromHours-double-) | Retourneert een TimeDelta die een opgegeven aantal uren vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Retourneert een TimeDelta die een opgegeven aantal milliseconden vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde). |
| [fromMinutes(double value)](#fromMinutes-double-) | Retourneert een TimeDelta die een opgegeven aantal minuten vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde). |
| [fromSeconds(double value)](#fromSeconds-double-) | Retourneert een TimeDelta die een opgegeven aantal seconden vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde). |
| [getDays()](#getDays--) | Retourneert het dagencomponent van het tijdsinterval, vertegenwoordigd door deze instantie. |
| [getHours()](#getHours--) | Retourneert het urencomponent van het tijdsinterval, vertegenwoordigd door deze instantie. |
| [getMilliseconds()](#getMilliseconds--) | Retourneert het millisecondencomponent van het tijdsinterval, vertegenwoordigd door deze instantie. |
| [getMinutes()](#getMinutes--) | Retourneert het minutencomponent van het tijdsinterval, vertegenwoordigd door deze instantie. |
| [getSeconds()](#getSeconds--) | Retourneert het secondencomponent van het tijdsinterval, vertegenwoordigd door deze instantie. |
| [getTotalDays()](#getTotalDays--) | Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele dagen. |
| [getTotalHours()](#getTotalHours--) | Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele uren. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele milliseconden. |
| [getTotalMinutes()](#getTotalMinutes--) | Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele minuten. |
| [getTotalSeconds()](#getTotalSeconds--) | Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele seconden. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Retourneert een nieuwe `TimeDelta` waarvan de waarde de negatie is van deze instantie. |
| [parse(String s)](#parse-java.lang.String-) | Converteert de tekenreeksrepresentatie van een tijdsinterval naar de overeenkomstige `TimeDelta`. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Retourneert een nieuw TimeDelta-object waarvan de waarde het verschil is tussen deze en `other` instanties. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Converteert de tekenreeksrepresentatie van een tijdsinterval naar de overeenkomstige TimeDelta en retourneert een waarde die aangeeft of de conversie geslaagd is. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Initialiseert een nieuwe instantie van TimeDelta met het opgegeven aantal uren, minuten en seconden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uren | int | aantal uren. |
| minuten | int | aantal minuten. |
| seconden | int | aantal seconden. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Initialiseert een nieuwe instantie van TimeDelta met het opgegeven aantal dagen, uren, minuten, seconden en milliseconden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dagen | int | aantal dagen. |
| uren | int | aantal uren. |
| minuten | int | aantal minuten. |
| seconden | int | aantal seconden. |
| milliseconden | int | aantal milliseconden. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Retourneert een nieuw TimeDelta-object waarvan de waarde de som is van deze en een andere instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | de instantie om mee op te tellen. |

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


Vergelijkt twee TimeDelta-waarden en retourneert een geheel getal dat aangeeft of de eerste waarde korter, gelijk aan of langer is dan de tweede waarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | het eerste tijdsinterval om te vergelijken. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | het tweede tijdsinterval om te vergelijken. |

**Returns:**
int - \-1 als `t1` korter is dan `t2`, 0 als `t1` gelijk is aan `t2` en 1 als `t1` langer is dan `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Vergelijkt deze instantie met een opgegeven TimeDelta-object en retourneert een geheel getal dat aangeeft of deze instantie korter, gelijk aan of langer is dan het TimeSpan-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | een instantie om mee te vergelijken. |

**Returns:**
int - \-1 als deze instantie korter is dan `other`, 0 als deze instantie gelijk is aan `other` en 1 als deze instantie langer is dan `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Geeft aan of een bepaalde `other` tijdsduur gelijk is aan deze.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | tijdspanne om mee te vergelijken. |

**Returns:**
boolean - `true` als intervallen gelijk zijn; `false` anders.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Controleert twee instanties op gelijkheid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | eerste instantie. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | tweede instantie. |

**Returns:**
boolean - `true` als instanties gelijk zijn; `false` anders.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| anders | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Retourneert een TimeDelta die een opgegeven aantal dagen vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een aantal dagen. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Retourneert een TimeDelta die een opgegeven aantal uren vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een aantal uren. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Retourneert een TimeDelta die een opgegeven aantal milliseconden vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een aantal milliseconden. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Retourneert een TimeDelta die een opgegeven aantal minuten vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een aantal minuten. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Retourneert een TimeDelta die een opgegeven aantal seconden vertegenwoordigt (afgerond op de dichtstbijzijnde milliseconde).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een aantal seconden. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Retourneert het dagencomponent van het tijdsinterval, vertegenwoordigd door deze instantie.

**Returns:**
int - het dagencomponent van het tijdsinterval. Kan positief of negatief zijn.
### getHours() {#getHours--}
```
public int getHours()
```


Retourneert het urencomponent van het tijdsinterval, vertegenwoordigd door deze instantie.

**Returns:**
int - het urencomponent van het tijdsinterval in het bereik van -23 tot en met 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Retourneert het millisecondencomponent van het tijdsinterval, vertegenwoordigd door deze instantie.

**Returns:**
int - het millisecondencomponent van het tijdsinterval in het bereik van -999 tot en met 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Retourneert het minutencomponent van het tijdsinterval, vertegenwoordigd door deze instantie.

**Returns:**
int - de minutencomponent van het tijdsinterval in bereik van -59 tot 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Retourneert het secondencomponent van het tijdsinterval, vertegenwoordigd door deze instantie.

**Returns:**
int - de secondencomponent van het tijdsinterval in bereik van -59 tot 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele dagen.

**Returns:**
double - het totale aantal dagen gerepresenteerd door deze instantie.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele uren.

**Returns:**
double - het totale aantal uren gerepresenteerd door deze instantie.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele milliseconden.

**Returns:**
double - het totale aantal milliseconden gerepresenteerd door deze instantie.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele minuten.

**Returns:**
double - het totale aantal minuten gerepresenteerd door deze instantie.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Retourneert de waarde van de huidige instantie uitgedrukt in gehele en fractionele seconden.

**Returns:**
double - het totale aantal seconden gerepresenteerd door deze instantie.
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


Retourneert een nieuwe `TimeDelta` waarvan de waarde de negatie is van deze instantie.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Converteert de tekenreeksrepresentatie van een tijdsinterval naar de overeenkomstige `TimeDelta`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| s | java.lang.String | een string die het tijdsinterval specificeert om te converteren. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Retourneert een nieuw TimeDelta-object waarvan de waarde het verschil is tussen deze en `other` instanties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | de instantie om af te trekken. |

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


Converteert de tekenreeksrepresentatie van een tijdsinterval naar de overeenkomstige TimeDelta en retourneert een waarde die aangeeft of de conversie geslaagd is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| s | java.lang.String | een string die het tijdsinterval specificeert om te converteren. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | deze array moet minstens één element bevatten. Wanneer deze methode terugkeert, bevat `result[0]` een object dat het tijdsinterval vertegenwoordigt dat door `s` is opgegeven, of een tijdsinterval met lengte nul als de conversie mislukt. |

**Returns:**
boolean - `true` als s succesvol is geconverteerd; anders `false`.
