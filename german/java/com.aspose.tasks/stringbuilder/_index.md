---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine veränderbare Zeichenkette dar."
type: docs
weight: 281
url: /de/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Stellt eine veränderbare Zeichenkette dar. Kann nicht erweitert werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Initialisiert eine neue Instanz der StringBuilder-Klasse. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Initialisiert eine neue Instanz der StringBuilder-Klasse mit der angegebenen Kapazität. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Initialisiert eine neue Instanz der StringBuilder-Klasse, die mit einer angegebenen Kapazität beginnt und bis zu einem angegebenen Maximum wachsen kann. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Initialisiert eine neue Instanz der StringBuilder-Klasse mit der angegebenen Zeichenkette. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Initialisiert eine neue Instanz der StringBuilder-Klasse mit der angegebenen Zeichenkette und Kapazität. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Initialisiert eine neue Instanz der StringBuilder-Klasse aus dem angegebenen Teilstring und der Kapazität. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Fügt die Zeichenkettenrepräsentation eines angegebenen booleschen Werts zu dieser Instanz hinzu. |
| [append(byte value)](#append-byte-) | Fügt die Zeichenkettenrepräsentation eines angegebenen Bytes zu dieser Instanz hinzu. |
| [append(char value)](#append-char-) | Fügt die Zeichenkettenrepräsentation eines angegebenen Unicode-Zeichens zu dieser Instanz hinzu. |
| [append(char value, int repeatCount)](#append-char-int-) | Fügt eine angegebene Anzahl von Kopien der Zeichenkettenrepräsentation eines Unicode-Zeichens zu dieser Instanz hinzu. |
| [append(char[] value)](#append-char---) | Fügt die Zeichenkettenrepräsentation der Unicode-Zeichen in einem angegebenen Array zu dieser Instanz hinzu. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Fügt die Zeichenkettenrepräsentation eines angegebenen Teilarrays von Unicode-Zeichen zu dieser Instanz hinzu. |
| [append(double value)](#append-double-) | Fügt die Zeichenkettenrepräsentation einer angegebenen double-Zahl zu dieser Instanz hinzu. |
| [append(float value)](#append-float-) | Fügt die Zeichenkettenrepräsentation einer angegebenen float-Zahl zu dieser Instanz hinzu. |
| [append(int value)](#append-int-) | Fügt die Zeichenkettenrepräsentation einer angegebenen int-Zahl zu dieser Instanz hinzu. |
| [append(Object value)](#append-java.lang.Object-) | Fügt die Zeichenkettenrepräsentation eines angegebenen Objekts zu dieser Instanz hinzu. |
| [append(String value)](#append-java.lang.String-) | Fügt eine Kopie der angegebenen Zeichenkette zu dieser Instanz hinzu. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Fügt eine Kopie eines angegebenen Teilstrings zu dieser Instanz hinzu. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Fügt die Zeichenkettenrepräsentation einer angegebenen BigDecimal-Zahl zu dieser Instanz hinzu. |
| [append(long value)](#append-long-) | Fügt die Zeichenkettenrepräsentation einer angegebenen long-Zahl zu dieser Instanz hinzu. |
| [append(short value)](#append-short-) | Fügt die Zeichenkettenrepräsentation einer angegebenen short-Zahl zu dieser Instanz hinzu. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Fügt die durch die Verarbeitung einer zusammengesetzten Formatzeichenkette zurückgegebene Zeichenkette, die null oder mehr Format-Elemente enthält, zu dieser Instanz hinzu. |
| [appendLine()](#appendLine--) | Fügt den Standardzeilenabschluss an das Ende des aktuellen StringBuilder-Objekts an. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Fügt eine Kopie der angegebenen Zeichenkette, gefolgt vom Standardzeilenabschluss, an das Ende des aktuellen StringBuilder-Objekts an. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Kopiert die Zeichen aus einem angegebenen Segment dieser Instanz in ein angegebenes Segment eines Ziel‑Char-Arrays. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Stellt sicher, dass die Kapazität dieser StringBuilder-Instanz mindestens den angegebenen Wert beträgt. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getCapacity()](#getCapacity--) | Ermittelt die maximale Anzahl von Zeichen, die im von der aktuellen Instanz zugewiesenen Speicher enthalten sein können. |
| [getLength()](#getLength--) | Ermittelt die Länge des aktuellen StringBuilder-Objekts. |
| [getMaxCapacity()](#getMaxCapacity--) | Ermittelt die maximale Kapazität dieser Instanz. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode für diesen StringBuilder zurück. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Fügt die Zeichenkettenrepräsentation eines booleschen Werts in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, byte value)](#insert-int-byte-) | Fügt die Zeichenkettenrepräsentation eines Byte‑Werts in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, char value)](#insert-int-char-) | Fügt die Zeichenkettenrepräsentation eines angegebenen Unicode‑Zeichens in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, char[] value)](#insert-int-char---) | Fügt die Zeichenkettenrepräsentation eines angegebenen Arrays von Unicode‑Zeichen in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Fügt die Zeichenkettenrepräsentation eines angegebenen Teilarrays von Unicode‑Zeichen in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, double value)](#insert-int-double-) | Fügt die Zeichenkettenrepräsentation einer double‑Zahl in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, float value)](#insert-int-float-) | Fügt die Zeichenkettenrepräsentation einer float‑Zahl in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, int value)](#insert-int-int-) | Fügt die Zeichenkettenrepräsentation einer int‑Zahl in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Fügt die Zeichenkettenrepräsentation eines Objekts in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Fügt eine Zeichenkette in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Fügt eine oder mehrere Kopien einer angegebenen Zeichenkette in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Fügt die Zeichenkettenrepräsentation einer Dezimalzahl in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, long value)](#insert-int-long-) | Fügt die Zeichenkettenrepräsentation einer long‑Zahl in diese Instanz an der angegebenen Zeichenposition ein. |
| [insert(int index, short value)](#insert-int-short-) | Fügt die Zeichenkettenrepräsentation einer short‑Zahl in diese Instanz an der angegebenen Zeichenposition ein. |
| [remove(int startIndex, int length)](#remove-int-int-) | Entfernt den angegebenen Zeichenbereich aus dieser Instanz. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Ersetzt alle Vorkommen eines angegebenen Zeichens in dieser Instanz durch ein anderes angegebenes Zeichen. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Ersetzt innerhalb eines Teilstrings dieser Instanz alle Vorkommen eines angegebenen Zeichens durch ein anderes angegebenes Zeichen. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Ersetzt alle Vorkommen einer angegebenen Zeichenkette in dieser Instanz durch eine andere angegebene Zeichenkette. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Ersetzt innerhalb eines Teilstrings dieser Instanz alle Vorkommen einer angegebenen Zeichenkette durch eine andere angegebene Zeichenkette. |
| [setCapacity(int value)](#setCapacity-int-) | Legt die maximale Anzahl von Zeichen fest, die im von der aktuellen Instanz zugewiesenen Speicher enthalten sein können. |
| [setLength(int value)](#setLength-int-) | Legt die Länge des aktuellen StringBuilder‑Objekts fest. |
| [toString()](#toString--) | Konvertiert den Wert dieser Instanz in eine Zeichenkette. |
| [toString(int startIndex, int length)](#toString-int-int-) | Konvertiert den Wert eines Teilstrings dieser Instanz in eine Zeichenkette. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Initialisiert eine neue Instanz der StringBuilder-Klasse.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Initialisiert eine neue Instanz der StringBuilder-Klasse mit der angegebenen Kapazität.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Kapazität | int | Die empfohlene Anfangsgröße dieser Instanz. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Initialisiert eine neue Instanz der StringBuilder-Klasse, die mit einer angegebenen Kapazität beginnt und bis zu einem angegebenen Maximum wachsen kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Kapazität | int | Die empfohlene Startgröße des StringBuilders. |
| maxCapacity | int | Die maximale Anzahl von Zeichen, die die aktuelle Zeichenkette enthalten kann. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Initialisiert eine neue Instanz der StringBuilder-Klasse mit der angegebenen Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Die Zeichenkette, die zum Initialisieren des Werts der Instanz verwendet wird. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Initialisiert eine neue Instanz der StringBuilder-Klasse mit der angegebenen Zeichenkette und Kapazität.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Die Zeichenkette, die zum Initialisieren des Werts der Instanz verwendet wird. |
| Kapazität | int | Die empfohlene Startgröße des StringBuilders. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Initialisiert eine neue Instanz der StringBuilder-Klasse aus dem angegebenen Teilstring und der Kapazität.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Die Zeichenkette, die die Teilzeichenkette enthält, die zum Initialisieren des Werts dieser Instanz verwendet wird. |
| startIndex | int | Die Position innerhalb des Werts, an der die Teilzeichenkette beginnt. |
| length | int | Die Anzahl der Zeichen in der Teilzeichenkette. |
| Kapazität | int | Die empfohlene Startgröße des StringBuilders. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen booleschen Werts zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Der boolesche Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen Bytes zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte | Der Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen Unicode-Zeichens zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char | Das Unicode-Zeichen, das angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Fügt eine angegebene Anzahl von Kopien der Zeichenkettenrepräsentation eines Unicode-Zeichens zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char | Das Zeichen, das angehängt werden soll. |
| repeatCount | int | Die Anzahl der Wiederholungen, um den Wert anzuhängen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Fügt die Zeichenkettenrepräsentation der Unicode-Zeichen in einem angegebenen Array zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char[] | Das Array von Zeichen, das angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen Teilarrays von Unicode-Zeichen zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char[] | Ein Zeichen-Array. |
| startIndex | int | Die Startposition im Wert. |
| charCount | int | Die Anzahl der Zeichen, die angehängt werden sollen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Fügt die Zeichenkettenrepräsentation einer angegebenen double-Zahl zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Der Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Fügt die Zeichenkettenrepräsentation einer angegebenen float-Zahl zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float | Der Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Fügt die Zeichenkettenrepräsentation einer angegebenen int-Zahl zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Der Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen Objekts zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Das Objekt, das angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Fügt eine Kopie der angegebenen Zeichenkette zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Die Zeichenkette zum Anhängen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Fügt eine Kopie eines angegebenen Teilstrings zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Die Zeichenkette, die die Teilzeichenkette zum Anhängen enthält. |
| startIndex | int | Die Startposition der Teilzeichenkette innerhalb des Werts. |
| Anzahl | int | Die Anzahl der Zeichen im Wert, die angehängt werden sollen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Fügt die Zeichenkettenrepräsentation einer angegebenen BigDecimal-Zahl zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | Der Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Fügt die Zeichenkettenrepräsentation einer angegebenen long-Zahl zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | long | Der Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Fügt die Zeichenkettenrepräsentation einer angegebenen short-Zahl zu dieser Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short | Der Wert, der angehängt werden soll. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Fügt die durch die Verarbeitung einer zusammengesetzten Formatzeichenkette zurückgegebene Zeichenkette an diese Instanz an. Jedes Formatitem wird durch die Zeichenkettenrepräsentation des entsprechenden Arguments in einem Parameterarray ersetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Format | java.lang.String | Eine zusammengesetzte Formatzeichenkette. |
| args | java.lang.Object[] | Ein Array von Objekten zum Formatieren. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Fügt den Standardzeilenabschluss an das Ende des aktuellen StringBuilder-Objekts an.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Fügt eine Kopie der angegebenen Zeichenkette, gefolgt vom Standardzeilenabschluss, an das Ende des aktuellen StringBuilder-Objekts an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Die Zeichenkette zum Anhängen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Kopiert die Zeichen aus einem angegebenen Segment dieser Instanz in ein angegebenes Segment eines Ziel‑Char-Arrays.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceIndex | int | Die Startposition in dieser Instanz, von der Zeichen kopiert werden. Der Index ist nullbasiert. |
| destination | char[] | Das Array, in das Zeichen kopiert werden. |
| destinationIndex | int | Die Startposition im Ziel, an die Zeichen kopiert werden. Der Index ist nullbasiert. |
| Anzahl | int | Die Anzahl der zu kopierenden Zeichen. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Stellt sicher, dass die Kapazität dieser StringBuilder-Instanz mindestens den angegebenen Wert beträgt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Kapazität | int | Die minimale Kapazität, die sichergestellt werden soll. |

**Returns:**
int – Die neue Kapazität dieser Instanz.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Ein Objekt zum Vergleich mit dieser Instanz oder null. |

**Returns:**
boolean – true, wenn diese Instanz und sb gleiche Zeichenkette, Kapazität und MaxKapazität‑Werte haben; andernfalls false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Ermittelt die maximale Anzahl von Zeichen, die im von der aktuellen Instanz zugewiesenen Speicher enthalten sein können.

**Returns:**
int – Die maximale Anzahl von Zeichen, die im von der aktuellen Instanz zugewiesenen Speicher enthalten sein können.
### getLength() {#getLength--}
```
public int getLength()
```


Ermittelt die Länge des aktuellen StringBuilder-Objekts.

**Returns:**
int – Die Länge dieser Instanz.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Ermittelt die maximale Kapazität dieser Instanz.

**Returns:**
int - Die maximale Anzahl von Zeichen, die diese Instanz halten kann.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode für diesen StringBuilder zurück.

**Returns:**
int - Gibt einen Hashcode-Wert für dieses Objekt zurück.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Fügt die Zeichenkettenrepräsentation eines booleschen Werts in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | boolean | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Fügt die Zeichenkettenrepräsentation eines Byte‑Werts in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | byte | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen Unicode‑Zeichens in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | char | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen Arrays von Unicode‑Zeichen in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | char[] | Das einzufügende Zeichenarray. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Fügt die Zeichenkettenrepräsentation eines angegebenen Teilarrays von Unicode‑Zeichen in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | char[] | Ein Zeichen-Array. |
| startIndex | int | Der Startindex innerhalb des Werts. |
| charCount | int | Die Anzahl der einzufügenden Zeichen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Fügt die Zeichenkettenrepräsentation einer double‑Zahl in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | double | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Fügt die Zeichenkettenrepräsentation einer float‑Zahl in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | float | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Fügt die Zeichenkettenrepräsentation einer int‑Zahl in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | int | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Fügt die Zeichenkettenrepräsentation eines Objekts in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | java.lang.Object | Das einzufügende Objekt oder null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Fügt eine Zeichenkette in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | java.lang.String | Die einzufügende Zeichenkette. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Fügt eine oder mehrere Kopien einer angegebenen Zeichenkette in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | java.lang.String | Die einzufügende Zeichenkette. |
| Anzahl | int | Die Anzahl der Wiederholungen, um den Wert einzufügen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Fügt die Zeichenkettenrepräsentation einer Dezimalzahl in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | java.math.BigDecimal | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Fügt die Zeichenkettenrepräsentation einer long‑Zahl in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | long | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Fügt die Zeichenkettenrepräsentation einer short‑Zahl in diese Instanz an der angegebenen Zeichenposition ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position in dieser Instanz, an der die Einfügung beginnt. |
| Wert | short | Der einzufügende Wert. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Entfernt den angegebenen Zeichenbereich aus dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Die nullbasierte Position in dieser Instanz, an der das Entfernen beginnt. |
| length | int | Die Anzahl der zu entfernenden Zeichen. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Ersetzt alle Vorkommen eines angegebenen Zeichens in dieser Instanz durch ein anderes angegebenes Zeichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldChar | char | Das zu ersetzende Zeichen. |
| newChar | char | Das Zeichen, das oldChar ersetzt. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Ersetzt innerhalb eines Teilstrings dieser Instanz alle Vorkommen eines angegebenen Zeichens durch ein anderes angegebenes Zeichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | char | Das zu ersetzende Zeichen. |
| newValue | char | Das Zeichen, das oldChar ersetzt. |
| startIndex | int | Die Position in dieser Instanz, an der die Teilzeichenkette beginnt. |
| Anzahl | int | Die Länge der Teilzeichenkette. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Ersetzt alle Vorkommen einer angegebenen Zeichenkette in dieser Instanz durch eine andere angegebene Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | java.lang.String | Die zu ersetzende Zeichenkette. |
| newValue | java.lang.String | Die Zeichenkette, die oldValue ersetzt, oder null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Ersetzt innerhalb eines Teilstrings dieser Instanz alle Vorkommen einer angegebenen Zeichenkette durch eine andere angegebene Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | java.lang.String | Die zu ersetzende Zeichenkette. |
| newValue | java.lang.String | Die Zeichenkette, die oldValue ersetzt, oder null. |
| startIndex | int | Die Position in dieser Instanz, an der die Teilzeichenkette beginnt. |
| Anzahl | int | Die Länge der Teilzeichenkette. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Legt die maximale Anzahl von Zeichen fest, die im von der aktuellen Instanz zugewiesenen Speicher enthalten sein können.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die maximale Anzahl von Zeichen, die im vom aktuellen Objekt zugewiesenen Speicher enthalten sein können. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Legt die Länge des aktuellen StringBuilder‑Objekts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Länge dieser Instanz. |

### toString() {#toString--}
```
public String toString()
```


Konvertiert den Wert dieser Instanz in eine Zeichenkette.

**Returns:**
java.lang.String - Eine Zeichenkette, deren Wert mit dieser Instanz identisch ist.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Konvertiert den Wert eines Teilstrings dieser Instanz in eine Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Die Startposition der Teilzeichenkette in dieser Instanz. |
| length | int | Die Länge der Teilzeichenkette. |

**Returns:**
java.lang.String - Eine Zeichenkette, deren Wert dem angegebenen Teilstring dieser Instanz entspricht.
