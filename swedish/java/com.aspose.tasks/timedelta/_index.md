---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en skillnad mellan två tidsstämplar."
type: docs
weight: 317
url: /sv/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Representerar en skillnad mellan två tidsstämplar.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Initierar en ny instans av TimeDelta till det angivna antalet timmar, minuter och sekunder. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Initierar en ny instans av TimeDelta till det angivna antalet dagar, timmar, minuter, sekunder och millisekunder. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Returnerar ett nytt TimeDelta-objekt vars värde är summan av denna och den andra instansen. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Jämför två TimeDelta-värden och returnerar ett heltal som indikerar om det första värdet är kortare än, lika med eller längre än det andra värdet. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Jämför den här instansen med ett specificerat TimeDelta-objekt och returnerar ett heltal som indikerar om den här instansen är kortare än, lika med eller längre än TimeSpan-objektet. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Indikerar om någon `other` tidsintervall är lika med denna. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Kontrollerar om två instanser är lika. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Returnerar en TimeDelta som representerar ett specificerat antal dagar (avrundat till närmaste millisekund). |
| [fromHours(double value)](#fromHours-double-) | Returnerar en TimeDelta som representerar ett specificerat antal timmar (avrundat till närmaste millisekund). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Returnerar en TimeDelta som representerar ett specificerat antal millisekunder (avrundat till närmaste millisekund). |
| [fromMinutes(double value)](#fromMinutes-double-) | Returnerar en TimeDelta som representerar ett specificerat antal minuter (avrundat till närmaste millisekund). |
| [fromSeconds(double value)](#fromSeconds-double-) | Returnerar en TimeDelta som representerar ett specificerat antal sekunder (avrundat till närmaste millisekund). |
| [getDays()](#getDays--) | Returnerar dagkomponenten i tidsintervallet som representeras av denna instans. |
| [getHours()](#getHours--) | Returnerar timkomponenten i tidsintervallet som representeras av denna instans. |
| [getMilliseconds()](#getMilliseconds--) | Returnerar millisekundkomponenten i tidsintervallet som representeras av denna instans. |
| [getMinutes()](#getMinutes--) | Returnerar minutkomponenten i tidsintervallet som representeras av denna instans. |
| [getSeconds()](#getSeconds--) | Returnerar sekundkomponenten i tidsintervallet som representeras av denna instans. |
| [getTotalDays()](#getTotalDays--) | Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av dagar. |
| [getTotalHours()](#getTotalHours--) | Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av timmar. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av millisekunder. |
| [getTotalMinutes()](#getTotalMinutes--) | Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av minuter. |
| [getTotalSeconds()](#getTotalSeconds--) | Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av sekunder. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Returnerar en ny `TimeDelta` vars värde är det negaterade värdet av denna instans. |
| [parse(String s)](#parse-java.lang.String-) | Konverterar strängrepresentationen av ett tidsintervall till dess `TimeDelta`-ekvivalent. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Returnerar ett nytt TimeDelta‑objekt vars värde är skillnaden mellan detta och `other`‑instanser. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Konverterar strängrepresentationen av ett tidsintervall till dess TimeDelta‑ekvivalent och returnerar ett värde som indikerar om konverteringen lyckades. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Initierar en ny instans av TimeDelta till det angivna antalet timmar, minuter och sekunder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| timmar | int | antal timmar. |
| minuter | int | antal minuter. |
| sekunder | int | antal sekunder. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Initierar en ny instans av TimeDelta till det angivna antalet dagar, timmar, minuter, sekunder och millisekunder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dagar | int | antal dagar. |
| timmar | int | antal timmar. |
| minuter | int | antal minuter. |
| sekunder | int | antal sekunder. |
| millisekunder | int | antal millisekunder. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Returnerar ett nytt TimeDelta-objekt vars värde är summan av denna och den andra instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | instansen att addera med. |

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


Jämför två TimeDelta-värden och returnerar ett heltal som indikerar om det första värdet är kortare än, lika med eller längre än det andra värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | det första tidsintervallet att jämföra. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | det andra tidsintervallet att jämföra. |

**Returns:**
int - \-1 om `t1` är kortare än `t2`, 0 om `t1` är lika med `t2` och 1 om `t1` är längre än `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Jämför den här instansen med ett specificerat TimeDelta-objekt och returnerar ett heltal som indikerar om den här instansen är kortare än, lika med eller längre än TimeSpan-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | en instans att jämföra med. |

**Returns:**
int - \-1 om denna instans är kortare än `other`, 0 om denna instans är lika med `other` och 1 om denna instans är längre än `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Indikerar om någon `other` tidsintervall är lika med denna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | tidsintervall att jämföra med. |

**Returns:**
boolean - `true` om intervallerna är lika; `false` annars.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Kontrollerar om två instanser är lika.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | första instansen. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | andra instansen. |

**Returns:**
boolean - `true` om instanserna är lika; `false` annars.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| annat | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Returnerar en TimeDelta som representerar ett specificerat antal dagar (avrundat till närmaste millisekund).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett antal dagar. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Returnerar en TimeDelta som representerar ett specificerat antal timmar (avrundat till närmaste millisekund).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett antal timmar. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Returnerar en TimeDelta som representerar ett specificerat antal millisekunder (avrundat till närmaste millisekund).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett antal millisekunder. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Returnerar en TimeDelta som representerar ett specificerat antal minuter (avrundat till närmaste millisekund).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett antal minuter. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Returnerar en TimeDelta som representerar ett specificerat antal sekunder (avrundat till närmaste millisekund).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett antal sekunder. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Returnerar dagkomponenten i tidsintervallet som representeras av denna instans.

**Returns:**
int - dagkomponenten i tidsintervallet. Kan vara positiv eller negativ.
### getHours() {#getHours--}
```
public int getHours()
```


Returnerar timkomponenten i tidsintervallet som representeras av denna instans.

**Returns:**
int - timkomponenten i tidsintervallet i intervallet från -23 till 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Returnerar millisekundkomponenten i tidsintervallet som representeras av denna instans.

**Returns:**
int - millisekundkomponenten i tidsintervallet i intervallet från -999 till 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Returnerar minutkomponenten i tidsintervallet som representeras av denna instans.

**Returns:**
int - minutkomponenten i tidsintervallet i intervallet från -59 till 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Returnerar sekundkomponenten i tidsintervallet som representeras av denna instans.

**Returns:**
int - sekundkomponenten i tidsintervallet i intervallet från -59 till 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av dagar.

**Returns:**
double - det totala antalet dagar som representeras av detta objekt.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av timmar.

**Returns:**
double - det totala antalet timmar som representeras av detta objekt.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av millisekunder.

**Returns:**
double - det totala antalet millisekunder som representeras av detta objekt.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av minuter.

**Returns:**
double - det totala antalet minuter som representeras av detta objekt.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Returnerar värdet av den aktuella instansen uttryckt i hela och bråkdelar av sekunder.

**Returns:**
double - det totala antalet sekunder som representeras av detta objekt.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int – \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


Returnerar en ny `TimeDelta` vars värde är det negaterade värdet av denna instans.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Konverterar strängrepresentationen av ett tidsintervall till dess `TimeDelta`-ekvivalent.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| s | java.lang.String | en sträng som specificerar tidsintervallet att konvertera. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Returnerar ett nytt TimeDelta‑objekt vars värde är skillnaden mellan detta och `other`‑instanser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | objektet att subtrahera. |

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


Konverterar strängrepresentationen av ett tidsintervall till dess TimeDelta‑ekvivalent och returnerar ett värde som indikerar om konverteringen lyckades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| s | java.lang.String | en sträng som specificerar tidsintervallet att konvertera. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | denna array måste ha minst ett element. När den här metoden returnerar, `result[0]` innehåller ett objekt som representerar tidsintervallet som specificerats av `s`, eller ett nollängds tidsintervall om konverteringen misslyckades. |

**Returns:**
boolean - `true` om s konverterades framgångsrikt; annars `false`.
