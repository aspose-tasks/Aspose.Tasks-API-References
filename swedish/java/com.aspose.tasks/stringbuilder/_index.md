---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en förändringsbar teckensträng."
type: docs
weight: 281
url: /sv/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Representerar en förändringsbar teckensträng. Kan inte utökas.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Initierar en ny instans av StringBuilder-klassen. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Initierar en ny instans av StringBuilder-klassen med den angivna kapaciteten. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Initierar en ny instans av StringBuilder-klassen som startar med en angiven kapacitet och kan växa till ett angivet maximum. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Initierar en ny instans av StringBuilder-klassen med den angivna strängen. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Initierar en ny instans av StringBuilder-klassen med den angivna strängen och kapaciteten. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Initierar en ny instans av StringBuilder-klassen från den angivna delsträngen och kapaciteten. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Lägger till strängrepresentationen av ett angivet booleskt värde till denna instans. |
| [append(byte value)](#append-byte-) | Lägger till strängrepresentationen av en angiven byte till denna instans. |
| [append(char value)](#append-char-) | Lägger till strängrepresentationen av ett angivet Unicode-tecken till denna instans. |
| [append(char value, int repeatCount)](#append-char-int-) | Lägger till ett angivet antal kopior av strängrepresentationen av ett Unicode-tecken till denna instans. |
| [append(char[] value)](#append-char---) | Lägger till strängrepresentationen av Unicode-tecknen i en specificerad array till detta objekt. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Lägger till strängrepresentationen av en specificerad delarray av Unicode-tecken till detta objekt. |
| [append(double value)](#append-double-) | Lägger till strängrepresentationen av ett specificerat double‑värde till detta objekt. |
| [append(float value)](#append-float-) | Lägger till strängrepresentationen av ett specificerat float‑värde till detta objekt. |
| [append(int value)](#append-int-) | Lägger till strängrepresentationen av ett specificerat int‑värde till detta objekt. |
| [append(Object value)](#append-java.lang.Object-) | Lägger till strängrepresentationen av ett specificerat objekt till detta objekt. |
| [append(String value)](#append-java.lang.String-) | Lägger till en kopia av den specificerade strängen till detta objekt. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Lägger till en kopia av en specificerad delsträng till detta objekt. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Lägger till strängrepresentationen av ett specificerat BigDecimal‑värde till detta objekt. |
| [append(long value)](#append-long-) | Lägger till strängrepresentationen av ett specificerat long‑värde till detta objekt. |
| [append(short value)](#append-short-) | Lägger till strängrepresentationen av ett specificerat short‑värde till detta objekt. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Lägger till den sträng som returneras genom att bearbeta en sammansatt formatsträng, som innehåller noll eller fler formatobjekt, till detta objekt. |
| [appendLine()](#appendLine--) | Lägger till standardradavslutaren i slutet av det aktuella StringBuilder‑objektet. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Lägger till en kopia av den specificerade strängen följt av standardradavslutaren i slutet av det aktuella StringBuilder‑objektet. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Kopierar tecknen från ett specificerat segment av detta objekt till ett specificerat segment av en mål‑Char‑array. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Säkerställer att kapaciteten för detta StringBuilder‑objekt är minst det specificerade värdet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getCapacity()](#getCapacity--) | Hämtar det maximala antalet tecken som kan lagras i minnet som tilldelats av det aktuella objektet. |
| [getLength()](#getLength--) | Hämtar längden på det aktuella StringBuilder‑objektet. |
| [getMaxCapacity()](#getMaxCapacity--) | Hämtar den maximala kapaciteten för detta objekt. |
| [hashCode()](#hashCode--) | Returnerar en hashkod för detta StringBuilder‑objekt. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Infogar strängrepresentationen av ett booleskt värde i detta objekt på den specificerade teckenpositionen. |
| [insert(int index, byte value)](#insert-int-byte-) | Infogar strängrepresentationen av ett byte‑värde i detta objekt på den specificerade teckenpositionen. |
| [insert(int index, char value)](#insert-int-char-) | Infogar strängrepresentationen av ett specificerat Unicode‑tecken i detta objekt på den specificerade teckenpositionen. |
| [insert(int index, char[] value)](#insert-int-char---) | Infogar strängrepresentationen av en specificerad array av Unicode‑tecken i detta objekt på den specificerade teckenpositionen. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Infogar strängrepresentationen av en specificerad delarray av Unicode‑tecken i detta objekt på den specificerade teckenpositionen. |
| [insert(int index, double value)](#insert-int-double-) | Infogar den strängrepresentationen av ett double‑tal i detta objekt på den angivna teckenpositionen. |
| [insert(int index, float value)](#insert-int-float-) | Infogar den strängrepresentationen av ett float‑tal i detta objekt på den angivna teckenpositionen. |
| [insert(int index, int value)](#insert-int-int-) | Infogar den strängrepresentationen av ett int‑tal i detta objekt på den angivna teckenpositionen. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Infogar den strängrepresentationen av ett objekt i detta objekt på den angivna teckenpositionen. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Infogar en sträng i detta objekt på den angivna teckenpositionen. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Infogar en eller flera kopior av en angiven sträng i detta objekt på den angivna teckenpositionen. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Infogar den strängrepresentationen av ett decimal‑tal i detta objekt på den angivna teckenpositionen. |
| [insert(int index, long value)](#insert-int-long-) | Infogar den strängrepresentationen av ett long‑tal i detta objekt på den angivna teckenpositionen. |
| [insert(int index, short value)](#insert-int-short-) | Infogar den strängrepresentationen av ett short‑tal i detta objekt på den angivna teckenpositionen. |
| [remove(int startIndex, int length)](#remove-int-int-) | Tar bort det angivna intervallet av tecken från detta objekt. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Ersätter alla förekomster av ett angivet tecken i detta objekt med ett annat angivet tecken. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Ersätter, inom en delsträng av detta objekt, alla förekomster av ett angivet tecken med ett annat angivet tecken. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Ersätter alla förekomster av en angiven sträng i detta objekt med en annan angiven sträng. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Ersätter, inom en delsträng av detta objekt, alla förekomster av en angiven sträng med en annan angiven sträng. |
| [setCapacity(int value)](#setCapacity-int-) | Anger det maximala antalet tecken som kan lagras i minnet som tilldelats det aktuella objektet. |
| [setLength(int value)](#setLength-int-) | Anger längden på det aktuella StringBuilder‑objektet. |
| [toString()](#toString--) | Konverterar värdet av detta objekt till en String. |
| [toString(int startIndex, int length)](#toString-int-int-) | Konverterar värdet av en delsträng av detta objekt till en String. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Initierar en ny instans av StringBuilder-klassen.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Initierar en ny instans av StringBuilder-klassen med den angivna kapaciteten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kapacitet | int | Den föreslagna startstorleken för detta objekt. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Initierar en ny instans av StringBuilder-klassen som startar med en angiven kapacitet och kan växa till ett angivet maximum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kapacitet | int | Den föreslagna startstorleken för StringBuilder. |
| maxCapacity | int | Det maximala antalet tecken som den aktuella strängen kan innehålla. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Initierar en ny instans av StringBuilder-klassen med den angivna strängen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Strängen som används för att initiera värdet av objektet. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Initierar en ny instans av StringBuilder-klassen med den angivna strängen och kapaciteten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Strängen som används för att initiera värdet av objektet. |
| kapacitet | int | Den föreslagna startstorleken för StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Initierar en ny instans av StringBuilder-klassen från den angivna delsträngen och kapaciteten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Strängen som innehåller delsträngen som används för att initiera värdet av detta objekt. |
| startIndex | int | Positionen inom value där delsträngen börjar. |
| length | int | Antalet tecken i delsträngen. |
| kapacitet | int | Den föreslagna startstorleken för StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Lägger till strängrepresentationen av ett angivet booleskt värde till denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | Det boolska värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Lägger till strängrepresentationen av en angiven byte till denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte | Värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Lägger till strängrepresentationen av ett angivet Unicode-tecken till denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char | Unicode-tecknet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Lägger till ett angivet antal kopior av strängrepresentationen av ett Unicode-tecken till denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char | Tecknet att lägga till. |
| repeatCount | int | Antalet gånger att lägga till value. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Lägger till strängrepresentationen av Unicode-tecknen i en specificerad array till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char[] | Arrayen av tecken att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Lägger till strängrepresentationen av en specificerad delarray av Unicode-tecken till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char[] | En teckenarray. |
| startIndex | int | Startpositionen i value. |
| charCount | int | Antalet tecken att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Lägger till strängrepresentationen av ett specificerat double‑värde till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | Värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Lägger till strängrepresentationen av ett specificerat float‑värde till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float | Värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Lägger till strängrepresentationen av ett specificerat int‑värde till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Lägger till strängrepresentationen av ett specificerat objekt till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | Objektet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Lägger till en kopia av den specificerade strängen till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Strängen att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Lägger till en kopia av en specificerad delsträng till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Strängen som innehåller delsträngen att lägga till. |
| startIndex | int | Startpositionen för delsträngen inom value. |
| count | int | Antalet tecken i value att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Lägger till strängrepresentationen av ett specificerat BigDecimal‑värde till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | Värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Lägger till strängrepresentationen av ett specificerat long‑värde till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | long | Värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Lägger till strängrepresentationen av ett specificerat short‑värde till detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short | Värdet att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Lägger till den sträng som returneras genom att bearbeta en sammansatt formatsträng, som innehåller noll eller fler formatobjekt, till detta objekt. Varje formatobjekt ersätts med strängrepresentationen av motsvarande argument i en parameterarray.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | java.lang.String | En sammansatt formatsträng. |
| args | java.lang.Object[] | En array av objekt att formatera. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Lägger till standardradavslutaren i slutet av det aktuella StringBuilder‑objektet.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Lägger till en kopia av den specificerade strängen följt av standardradavslutaren i slutet av det aktuella StringBuilder‑objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Strängen att lägga till. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Kopierar tecknen från ett specificerat segment av detta objekt till ett specificerat segment av en mål‑Char‑array.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceIndex | int | Startpositionen i detta objekt varifrån tecken kommer att kopieras. Indexet är nollbaserat. |
| destination | char[] | Arrayen där tecken kommer att kopieras. |
| destinationIndex | int | Startpositionen i destinationen där tecken kommer att kopieras. Indexet är nollbaserat. |
| count | int | Antalet tecken som ska kopieras. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Säkerställer att kapaciteten för detta StringBuilder‑objekt är minst det specificerade värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kapacitet | int | Den minsta kapaciteten att säkerställa. |

**Returns:**
int - Den nya kapaciteten för detta objekt.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Ett objekt att jämföra med detta objekt, eller null. |

**Returns:**
boolean - true om detta objekt och sb har lika string, Capacity och MaxCapacity värden; annars false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Hämtar det maximala antalet tecken som kan lagras i minnet som tilldelats av det aktuella objektet.

**Returns:**
int - Det maximala antalet tecken som kan rymmas i minnet som allokerats av det aktuella objektet.
### getLength() {#getLength--}
```
public int getLength()
```


Hämtar längden på det aktuella StringBuilder‑objektet.

**Returns:**
int - Längden på detta objekt.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Hämtar den maximala kapaciteten för detta objekt.

**Returns:**
int - Det maximala antalet tecken som detta objekt kan innehålla.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar en hashkod för detta StringBuilder‑objekt.

**Returns:**
int - Returnerar ett hashkodsvärde för detta objekt.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Infogar strängrepresentationen av ett booleskt värde i detta objekt på den specificerade teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | boolean | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Infogar strängrepresentationen av ett byte‑värde i detta objekt på den specificerade teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | byte | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Infogar strängrepresentationen av ett specificerat Unicode‑tecken i detta objekt på den specificerade teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | char | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Infogar strängrepresentationen av en specificerad array av Unicode‑tecken i detta objekt på den specificerade teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | char[] | Teckenarrayen att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Infogar strängrepresentationen av en specificerad delarray av Unicode‑tecken i detta objekt på den specificerade teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | char[] | En teckenarray. |
| startIndex | int | Startindexet inom värdet. |
| charCount | int | Antalet tecken att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Infogar den strängrepresentationen av ett double‑tal i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | double | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Infogar den strängrepresentationen av ett float‑tal i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | float | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Infogar den strängrepresentationen av ett int‑tal i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | int | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Infogar den strängrepresentationen av ett objekt i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | java.lang.Object | Objektet att infoga, eller null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Infogar en sträng i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | java.lang.String | Strängen att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Infogar en eller flera kopior av en angiven sträng i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | java.lang.String | Strängen att infoga. |
| count | int | Antalet gånger värdet ska infogas. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Infogar den strängrepresentationen av ett decimal‑tal i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | java.math.BigDecimal | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Infogar den strängrepresentationen av ett long‑tal i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | long | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Infogar den strängrepresentationen av ett short‑tal i detta objekt på den angivna teckenpositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen i detta objekt där insättningen börjar. |
| värde | short | Värdet att infoga. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Tar bort det angivna intervallet av tecken från detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Den nollbaserade positionen i detta objekt där borttagning börjar. |
| length | int | Antalet tecken att ta bort. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Ersätter alla förekomster av ett angivet tecken i detta objekt med ett annat angivet tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldChar | char | Tecknet att ersätta. |
| newChar | char | Tecknet som ersätter oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Ersätter, inom en delsträng av detta objekt, alla förekomster av ett angivet tecken med ett annat angivet tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | char | Tecknet att ersätta. |
| newValue | char | Tecknet som ersätter oldChar. |
| startIndex | int | Positionen i detta objekt där delsträngen börjar. |
| count | int | Längden på delsträngen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Ersätter alla förekomster av en angiven sträng i detta objekt med en annan angiven sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | java.lang.String | Strängen att ersätta. |
| newValue | java.lang.String | Strängen som ersätter oldValue, eller null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Ersätter, inom en delsträng av detta objekt, alla förekomster av en angiven sträng med en annan angiven sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | java.lang.String | Strängen att ersätta. |
| newValue | java.lang.String | Strängen som ersätter oldValue, eller null. |
| startIndex | int | Positionen i detta objekt där delsträngen börjar. |
| count | int | Längden på delsträngen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Anger det maximala antalet tecken som kan lagras i minnet som tilldelats det aktuella objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Det maximala antalet tecken som kan finnas i minnet som allokerats av det aktuella objektet. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Anger längden på det aktuella StringBuilder‑objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Längden på detta objekt. |

### toString() {#toString--}
```
public String toString()
```


Konverterar värdet av detta objekt till en String.

**Returns:**
java.lang.String - En sträng vars värde är detsamma som detta objekt.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Konverterar värdet av en delsträng av detta objekt till en String.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Startpositionen för delsträngen i detta objekt. |
| length | int | Längden på delsträngen. |

**Returns:**
java.lang.String - En sträng vars värde är detsamma som den angivna delsträngen i detta objekt.
