---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung von Objekten dar."
type: docs
weight: 321
url: /de/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

Stellt eine Sammlung von [TimephasedData](../../com.aspose.tasks/timephaseddata)-Objekten dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | Initialisiert eine neue Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | Fügt eine [TimephasedData](../../com.aspose.tasks/timephaseddata)-Instanz zu diesem Sammlungsobjekt hinzu. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | Fügt eine Sammlung von [TimephasedData](../../com.aspose.tasks/timephaseddata)-Instanzen zu diesem Sammlungsobjekt hinzu. |
| [clear()](#clear--) | Entfernt alle Elemente aus der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | Bestimmt, ob die [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) einen bestimmten Wert enthält. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | Kopiert die Elemente der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in ein Array, beginnend bei einem bestimmten Array-Index. |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Gibt einen Wert zurück, der angibt, ob die System.Collections.Generic.ICollection&lt;T&gt; schreibgeschützt ist. |
| [iterator()](#iterator--) | Gibt einen Iterator für diese Sammlung zurück. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | Entfernt die [TimephasedData](../../com.aspose.tasks/timephaseddata)-Instanz aus diesem Sammlungsobjekt. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | Wählt alle Zeitphasen zwischen `startTime` und `finishTime` aus. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | Setzt das Element am angegebenen Index. |
| [size()](#size--) | Gibt die Anzahl der in diesem [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Objekt enthaltenen Objekte zurück. |
| [toList()](#toList--) | Konvertiert das [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Objekt in eine Liste von [TimephasedData](../../com.aspose.tasks/timephaseddata)-Objekten. |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


Initialisiert eine neue Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


Fügt eine [TimephasedData](../../com.aspose.tasks/timephaseddata)-Instanz zu diesem Sammlungsobjekt hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Das hinzuzufügende Element. |

**Returns:**
boolean - true, wenn das Element hinzugefügt wurde; andernfalls false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


Fügt eine Sammlung von [TimephasedData](../../com.aspose.tasks/timephaseddata)-Instanzen zu diesem Sammlungsobjekt hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | Eine Sammlung von [TimephasedData](../../com.aspose.tasks/timephaseddata)-Objekten zum Hinzufügen. |

### clear() {#clear--}
```
public final void clear()
```


Entfernt alle Elemente aus der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


Bestimmt, ob die [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) einen bestimmten Wert enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Das Objekt, das in der Sammlung gefunden werden soll. |

**Returns:**
boolean - true, wenn `item` in der Sammlung gefunden wird; andernfalls false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


Kopiert die Elemente der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in ein Array, beginnend bei einem bestimmten Array-Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | Das eindimensionale Array, das das Ziel der aus [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) kopierten Elemente ist. Das Array muss nullbasierte Indizierung besitzen. |
| arrayIndex | int | Der nullbasierte Index in `array`, bei dem das Kopieren beginnt. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Gibt einen Wert zurück, der angibt, ob die System.Collections.Generic.ICollection&lt;T&gt; schreibgeschützt ist.

**Returns:**
boolean - true, wenn die System.Collections.Generic.ICollection&lt;T&gt; schreibgeschützt ist; andernfalls false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


Gibt einen Iterator für diese Sammlung zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.TimephasedData&gt; - ein Iterator für diese Sammlung.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


Entfernt die [TimephasedData](../../com.aspose.tasks/timephaseddata)-Instanz aus diesem Sammlungsobjekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Das zu entfernende Element. |

**Returns:**
boolean - true, wenn `item` erfolgreich aus der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) entfernt wurde; andernfalls false. Diese Methode gibt ebenfalls false zurück, wenn `item` in der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) nicht gefunden wird.
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


Wählt alle Zeitphasen zwischen `startTime` und `finishTime` aus. Hat im Durchschnitt O(log n)-Komplexität.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| timephasedDataType | byte | Typ der auszuwählenden Zeitphasen. |
| startTime | java.util.Date | Start des Intervalls. |
| finishTime | java.util.Date | Ende des Intervalls. |

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Gibt eine neue List-Instanz der Daten aus [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) zurück, sortiert nach der Start-Eigenschaft.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


Setzt das Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des zu setzenden Elements. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | das Element, das gesetzt werden soll. |

### size() {#size--}
```
public final int size()
```


Gibt die Anzahl der in diesem [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Objekt enthaltenen Objekte zurück.

**Returns:**
int - die Anzahl der Objekte, die in diesem [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) Objekt enthalten sind.
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


Konvertiert das [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Objekt in eine Liste von [TimephasedData](../../com.aspose.tasks/timephaseddata)-Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Liste von [TimephasedData](../../com.aspose.tasks/timephaseddata) Objekten.
