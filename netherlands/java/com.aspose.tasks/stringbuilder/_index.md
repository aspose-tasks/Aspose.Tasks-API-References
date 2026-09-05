---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een wijzigbare tekenreeks voor."
type: docs
weight: 281
url: /nl/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Stelt een wijzigbare tekenreeks van karakters voor. Kan niet worden uitgebreid.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Initialiseert een nieuw exemplaar van de StringBuilder-klasse. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Initialiseert een nieuw exemplaar van de StringBuilder-klasse met de opgegeven capaciteit. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Initialiseert een nieuw exemplaar van de StringBuilder-klasse dat begint met een opgegeven capaciteit en kan groeien tot een opgegeven maximum. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Initialiseert een nieuw exemplaar van de StringBuilder-klasse met de opgegeven tekenreeks. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Initialiseert een nieuw exemplaar van de StringBuilder-klasse met de opgegeven tekenreeks en capaciteit. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Initialiseert een nieuw exemplaar van de StringBuilder-klasse vanuit de opgegeven subtekenreeks en capaciteit. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Voegt de tekenreeksrepresentatie van een opgegeven booleaanse waarde toe aan dit exemplaar. |
| [append(byte value)](#append-byte-) | Voegt de tekenreeksrepresentatie van een opgegeven byte toe aan dit exemplaar. |
| [append(char value)](#append-char-) | Voegt de tekenreeksrepresentatie van een opgegeven Unicode‑teken toe aan dit exemplaar. |
| [append(char value, int repeatCount)](#append-char-int-) | Voegt een opgegeven aantal kopieën van de tekenreeksrepresentatie van een Unicode‑teken toe aan dit exemplaar. |
| [append(char[] value)](#append-char---) | Voegt de tekenreeksrepresentatie van de Unicode‑tekens in een opgegeven array toe aan dit exemplaar. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Voegt de tekenreeksrepresentatie van een opgegeven subarray van Unicode‑tekens toe aan dit exemplaar. |
| [append(double value)](#append-double-) | Voegt de tekenreeksrepresentatie van een opgegeven double‑getal toe aan dit exemplaar. |
| [append(float value)](#append-float-) | Voegt de tekenreeksrepresentatie van een opgegeven float‑getal toe aan dit exemplaar. |
| [append(int value)](#append-int-) | Voegt de tekenreeksrepresentatie van een opgegeven int‑getal toe aan dit exemplaar. |
| [append(Object value)](#append-java.lang.Object-) | Voegt de tekenreeksrepresentatie van een opgegeven object toe aan dit exemplaar. |
| [append(String value)](#append-java.lang.String-) | Voegt een kopie van de opgegeven tekenreeks toe aan dit exemplaar. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Voegt een kopie van een opgegeven subtekenreeks toe aan dit exemplaar. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Voegt de tekenreeksrepresentatie van een opgegeven BigDecimal‑getal toe aan dit exemplaar. |
| [append(long value)](#append-long-) | Voegt de tekenreeksrepresentatie van een opgegeven long‑getal toe aan deze instantie. |
| [append(short value)](#append-short-) | Voegt de tekenreeksrepresentatie van een opgegeven short‑getal toe aan deze instantie. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Voegt de tekenreeks toe die wordt geretourneerd door het verwerken van een samengestelde opmaaktekenreeks, die nul of meer opmaakitems bevat, aan deze instantie. |
| [appendLine()](#appendLine--) | Voegt de standaard regeleinde‑terminator toe aan het einde van het huidige StringBuilder‑object. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Voegt een kopie van de opgegeven tekenreeks, gevolgd door de standaard regeleinde‑terminator, toe aan het einde van het huidige StringBuilder‑object. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Kopieert de tekens van een opgegeven segment van deze instantie naar een opgegeven segment van een doel‑Char‑array. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Zorgt ervoor dat de capaciteit van deze StringBuilder‑instantie ten minste de opgegeven waarde is. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getCapacity()](#getCapacity--) | Haalt het maximale aantal tekens op dat kan worden opgeslagen in het geheugen dat door de huidige instantie is toegewezen. |
| [getLength()](#getLength--) | Haalt de lengte op van het huidige StringBuilder‑object. |
| [getMaxCapacity()](#getMaxCapacity--) | Haalt de maximale capaciteit van deze instantie op. |
| [hashCode()](#hashCode--) | Retourneert een hash‑code voor deze StringBuilder. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Voegt de tekenreeksrepresentatie van een booleaanse waarde in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, byte value)](#insert-int-byte-) | Voegt de tekenreeksrepresentatie van een byte‑waarde in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, char value)](#insert-int-char-) | Voegt de tekenreeksrepresentatie van een opgegeven Unicode‑teken in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, char[] value)](#insert-int-char---) | Voegt de tekenreeksrepresentatie van een opgegeven array van Unicode‑tekens in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Voegt de tekenreeksrepresentatie van een opgegeven subarray van Unicode‑tekens in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, double value)](#insert-int-double-) | Voegt de tekenreeksrepresentatie van een double‑getal in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, float value)](#insert-int-float-) | Voegt de tekenreeksrepresentatie van een float‑getal in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, int value)](#insert-int-int-) | Voegt de tekenreeksrepresentatie van een int‑getal in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Voegt de tekenreeksrepresentatie van een object in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Voegt een tekenreeks in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Voegt een of meer kopieën van een opgegeven tekenreeks in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Voegt de tekenreeksrepresentatie van een decimaal‑getal in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, long value)](#insert-int-long-) | Voegt de tekenreeksrepresentatie van een long‑getal in deze instantie in op de opgegeven tekenpositie. |
| [insert(int index, short value)](#insert-int-short-) | Voegt de tekenreeksrepresentatie van een short‑getal in deze instantie in op de opgegeven tekenpositie. |
| [remove(int startIndex, int length)](#remove-int-int-) | Verwijdert het opgegeven bereik van tekens uit deze instantie. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Vervangt alle voorkomens van een opgegeven teken in deze instantie door een ander opgegeven teken. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Vervangt, binnen een substring van deze instantie, alle voorkomens van een opgegeven teken door een ander opgegeven teken. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Vervangt alle voorkomens van een opgegeven tekenreeks in deze instantie door een andere opgegeven tekenreeks. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Vervangt, binnen een substring van deze instantie, alle voorkomens van een opgegeven tekenreeks door een andere opgegeven tekenreeks. |
| [setCapacity(int value)](#setCapacity-int-) | Stelt het maximale aantal tekens in dat kan worden opgeslagen in het geheugen dat door de huidige instantie is toegewezen. |
| [setLength(int value)](#setLength-int-) | Stelt de lengte in van het huidige StringBuilder-object. |
| [toString()](#toString--) | Converteert de waarde van deze instantie naar een String. |
| [toString(int startIndex, int length)](#toString-int-int-) | Converteert de waarde van een substring van deze instantie naar een String. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Initialiseert een nieuw exemplaar van de StringBuilder-klasse.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Initialiseert een nieuw exemplaar van de StringBuilder-klasse met de opgegeven capaciteit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| capaciteit | int | De voorgestelde begingrootte van deze instantie. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Initialiseert een nieuw exemplaar van de StringBuilder-klasse dat begint met een opgegeven capaciteit en kan groeien tot een opgegeven maximum.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| capaciteit | int | De voorgestelde begingrootte van de StringBuilder. |
| maxCapacity | int | Het maximale aantal tekens dat de huidige string kan bevatten. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Initialiseert een nieuw exemplaar van de StringBuilder-klasse met de opgegeven tekenreeks.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De tekenreeks die wordt gebruikt om de waarde van de instantie te initialiseren. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Initialiseert een nieuw exemplaar van de StringBuilder-klasse met de opgegeven tekenreeks en capaciteit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De tekenreeks die wordt gebruikt om de waarde van de instantie te initialiseren. |
| capaciteit | int | De voorgestelde begingrootte van de StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Initialiseert een nieuw exemplaar van de StringBuilder-klasse vanuit de opgegeven subtekenreeks en capaciteit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De tekenreeks die de substring bevat die wordt gebruikt om de waarde van deze instantie te initialiseren. |
| startIndex | int | De positie binnen de waarde waar de substring begint. |
| length | int | Het aantal tekens in de substring. |
| capaciteit | int | De voorgestelde begingrootte van de StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Voegt de tekenreeksrepresentatie van een opgegeven booleaanse waarde toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | De booleaanse waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Voegt de tekenreeksrepresentatie van een opgegeven byte toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | byte | De waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Voegt de tekenreeksrepresentatie van een opgegeven Unicode‑teken toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | char | Het Unicode-teken om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Voegt een opgegeven aantal kopieën van de tekenreeksrepresentatie van een Unicode‑teken toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | char | Het teken om toe te voegen. |
| repeatCount | int | Het aantal keren dat de waarde moet worden toegevoegd. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Voegt de tekenreeksrepresentatie van de Unicode‑tekens in een opgegeven array toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | char[] | De array van tekens om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Voegt de tekenreeksrepresentatie van een opgegeven subarray van Unicode‑tekens toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | char[] | Een tekenarray. |
| startIndex | int | De beginnende positie in de waarde. |
| charCount | int | Het aantal tekens om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Voegt de tekenreeksrepresentatie van een opgegeven double‑getal toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | De waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Voegt de tekenreeksrepresentatie van een opgegeven float‑getal toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float | De waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Voegt de tekenreeksrepresentatie van een opgegeven int‑getal toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | De waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Voegt de tekenreeksrepresentatie van een opgegeven object toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.Object | Het object om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Voegt een kopie van de opgegeven tekenreeks toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De string om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Voegt een kopie van een opgegeven subtekenreeks toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De string die de substring bevat die moet worden toegevoegd. |
| startIndex | int | De beginnende positie van de substring binnen de waarde. |
| count | int | Het aantal tekens in de waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Voegt de tekenreeksrepresentatie van een opgegeven BigDecimal‑getal toe aan dit exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | De waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Voegt de tekenreeksrepresentatie van een opgegeven long‑getal toe aan deze instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | long | De waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Voegt de tekenreeksrepresentatie van een opgegeven short‑getal toe aan deze instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | short | De waarde om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Voegt de string toe die wordt geretourneerd door het verwerken van een samengestelde opmaakstring, die nul of meer opmaakitems bevat, aan deze instantie. Elk opmaakitem wordt vervangen door de tekenreeksrepresentatie van een overeenkomstig argument in een parameterarray.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| format | java.lang.String | Een samengestelde opmaakstring. |
| args | java.lang.Object[] | Een array van objecten om op te maken. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Voegt de standaard regeleinde‑terminator toe aan het einde van het huidige StringBuilder‑object.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Voegt een kopie van de opgegeven tekenreeks, gevolgd door de standaard regeleinde‑terminator, toe aan het einde van het huidige StringBuilder‑object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De string om toe te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Kopieert de tekens van een opgegeven segment van deze instantie naar een opgegeven segment van een doel‑Char‑array.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceIndex | int | De beginnende positie in deze instantie waar tekens vandaan gekopieerd worden. De index is nulgebaseerd. |
| destination | char[] | De array waarin tekens worden gekopieerd. |
| destinationIndex | int | De startpositie in destination waar tekens worden gekopieerd. De index is nulgebaseerd. |
| count | int | Het aantal tekens dat gekopieerd moet worden. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Zorgt ervoor dat de capaciteit van deze StringBuilder‑instantie ten minste de opgegeven waarde is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| capaciteit | int | De minimale capaciteit om te waarborgen. |

**Returns:**
int - De nieuwe capaciteit van deze instantie.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Een object om te vergelijken met deze instantie, of null. |

**Returns:**
boolean - true als deze instantie en sb gelijke string-, Capacity- en MaxCapacity-waarden hebben; anders false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Haalt het maximale aantal tekens op dat kan worden opgeslagen in het geheugen dat door de huidige instantie is toegewezen.

**Returns:**
int - Het maximale aantal tekens dat kan worden opgeslagen in het geheugen dat door de huidige instantie is toegewezen.
### getLength() {#getLength--}
```
public int getLength()
```


Haalt de lengte op van het huidige StringBuilder‑object.

**Returns:**
int - De lengte van deze instantie.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Haalt de maximale capaciteit van deze instantie op.

**Returns:**
int - Het maximale aantal tekens dat deze instantie kan bevatten.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hash‑code voor deze StringBuilder.

**Returns:**
int - Retourneert een hashcode-waarde voor dit object.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Voegt de tekenreeksrepresentatie van een booleaanse waarde in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | boolean | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Voegt de tekenreeksrepresentatie van een byte‑waarde in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | byte | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Voegt de tekenreeksrepresentatie van een opgegeven Unicode‑teken in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | char | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Voegt de tekenreeksrepresentatie van een opgegeven array van Unicode‑tekens in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | char[] | De tekenarray om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Voegt de tekenreeksrepresentatie van een opgegeven subarray van Unicode‑tekens in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | char[] | Een tekenarray. |
| startIndex | int | De startindex binnen waarde. |
| charCount | int | Het aantal tekens om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Voegt de tekenreeksrepresentatie van een double‑getal in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | double | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Voegt de tekenreeksrepresentatie van een float‑getal in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | float | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Voegt de tekenreeksrepresentatie van een int‑getal in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | int | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Voegt de tekenreeksrepresentatie van een object in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | java.lang.Object | Het object om in te voegen, of null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Voegt een tekenreeks in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | java.lang.String | De string om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Voegt een of meer kopieën van een opgegeven tekenreeks in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | java.lang.String | De string om in te voegen. |
| count | int | Het aantal keren dat de waarde moet worden ingevoegd. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Voegt de tekenreeksrepresentatie van een decimaal‑getal in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | java.math.BigDecimal | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Voegt de tekenreeksrepresentatie van een long‑getal in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | long | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Voegt de tekenreeksrepresentatie van een short‑getal in deze instantie in op de opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De positie in deze instantie waar de invoeging begint. |
| waarde | short | De waarde om in te voegen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Verwijdert het opgegeven bereik van tekens uit deze instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| startIndex | int | De nulgebaseerde positie in deze instantie waar het verwijderen begint. |
| length | int | Het aantal tekens om te verwijderen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Vervangt alle voorkomens van een opgegeven teken in deze instantie door een ander opgegeven teken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldChar | char | Het teken om te vervangen. |
| newChar | char | Het teken dat oldChar vervangt. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Vervangt, binnen een substring van deze instantie, alle voorkomens van een opgegeven teken door een ander opgegeven teken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldValue | char | Het teken om te vervangen. |
| newValue | char | Het teken dat oldChar vervangt. |
| startIndex | int | De positie in deze instantie waar de subreeks begint. |
| count | int | De lengte van de subreeks. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Vervangt alle voorkomens van een opgegeven tekenreeks in deze instantie door een andere opgegeven tekenreeks.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldValue | java.lang.String | De te vervangen tekenreeks. |
| newValue | java.lang.String | De tekenreeks die oldValue vervangt, of null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Vervangt, binnen een substring van deze instantie, alle voorkomens van een opgegeven tekenreeks door een andere opgegeven tekenreeks.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldValue | java.lang.String | De te vervangen tekenreeks. |
| newValue | java.lang.String | De tekenreeks die oldValue vervangt, of null. |
| startIndex | int | De positie in deze instantie waar de subreeks begint. |
| count | int | De lengte van de subreeks. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Stelt het maximale aantal tekens in dat kan worden opgeslagen in het geheugen dat door de huidige instantie is toegewezen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | Het maximale aantal tekens dat kan worden opgeslagen in het geheugen dat door de huidige instantie is toegewezen. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Stelt de lengte in van het huidige StringBuilder-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | De lengte van deze instantie. |

### toString() {#toString--}
```
public String toString()
```


Converteert de waarde van deze instantie naar een String.

**Returns:**
java.lang.String - Een tekenreeks waarvan de waarde gelijk is aan deze instantie.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Converteert de waarde van een substring van deze instantie naar een String.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| startIndex | int | De startpositie van de subreeks in deze instantie. |
| length | int | De lengte van de subreeks. |

**Returns:**
java.lang.String - Een tekenreeks waarvan de waarde gelijk is aan de opgegeven subreeks van deze instantie.
