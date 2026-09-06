---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling av  objekt."
type: docs
weight: 321
url: /sv/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

Representerar en samling av [TimephasedData](../../com.aspose.tasks/timephaseddata) objekt.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | Initierar en ny instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | Lägger till en [TimephasedData](../../com.aspose.tasks/timephaseddata)-instans till detta samlingsobjekt. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | Lägger till en samling av [TimephasedData](../../com.aspose.tasks/timephaseddata)-instanser till detta samlingsobjekt. |
| [clear()](#clear--) | Tar bort alla objekt från [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | Bestämmer om [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) innehåller ett specifikt värde. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | Kopierar elementen i [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) till en Array, med start vid ett specifikt Array-index. |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Hämtar ett värde som indikerar om System.Collections.Generic.ICollection&lt;T&gt; är skrivskyddad. |
| [iterator()](#iterator--) | Returnerar en iterator för denna samling. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | Tar bort en [TimephasedData](../../com.aspose.tasks/timephaseddata)-instans från detta samlingsobjekt. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | Väljer alla tidsfaser mellan `startTime` och `finishTime`. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | Ställer in elementet på det angivna indexet. |
| [size()](#size--) | Hämtar antalet objekt som finns i detta [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) objekt. |
| [toList()](#toList--) | Konverterar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) objektet till en lista med [TimephasedData](../../com.aspose.tasks/timephaseddata) objekt. |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


Initierar en ny instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


Lägger till en [TimephasedData](../../com.aspose.tasks/timephaseddata)-instans till detta samlingsobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Objektet att lägga till. |

**Returns:**
boolean - true, om item lades till; annars false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


Lägger till en samling av [TimephasedData](../../com.aspose.tasks/timephaseddata)-instanser till detta samlingsobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | En samling av [TimephasedData](../../com.aspose.tasks/timephaseddata) objekt att lägga till. |

### clear() {#clear--}
```
public final void clear()
```


Tar bort alla objekt från [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


Bestämmer om [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) innehåller ett specifikt värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Objektet att hitta i samlingen. |

**Returns:**
boolean - true om `item` hittas i samlingen; annars false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


Kopierar elementen i [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) till en Array, med start vid ett specifikt Array-index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | Den endimensionella arrayen som är destinationen för elementen som kopierats från [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). Arrayen måste ha nollbaserad indexering. |
| arrayIndex | int | Det nollbaserade indexet i `array` där kopieringen börjar. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Hämtar ett värde som indikerar om System.Collections.Generic.ICollection&lt;T&gt; är skrivskyddad.

**Returns:**
boolean - true om System.Collections.Generic.ICollection&lt;T&gt; är skrivskyddad; annars false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


Returnerar en iterator för denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.TimephasedData&gt; - en iterator för denna samling.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


Tar bort en [TimephasedData](../../com.aspose.tasks/timephaseddata)-instans från detta samlingsobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Objektet som ska tas bort. |

**Returns:**
boolean - true om `item` framgångsrikt togs bort från [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection); annars false. Denna metod returnerar också false om `item` inte hittas i [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


Väljer alla tidsfaser mellan `startTime` och `finishTime`. Har O(log n) komplexitet i genomsnittligt fall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| timephasedDataType | byte | Typ av tidsfaser att välja. |
| startTime | java.util.Date | Intervallets start. |
| finishTime | java.util.Date | Intervallets slut. |

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Returnerar en ny listinstans av [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) data sorterade efter egenskapen Start.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


Ställer in elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet som ska sättas. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | elementet att sätta. |

### size() {#size--}
```
public final int size()
```


Hämtar antalet objekt som finns i detta [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) objekt.

**Returns:**
int - antalet objekt som finns i detta [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) objekt.
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


Konverterar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) objektet till en lista med [TimephasedData](../../com.aspose.tasks/timephaseddata) objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Lista med [TimephasedData](../../com.aspose.tasks/timephaseddata) objekt.
