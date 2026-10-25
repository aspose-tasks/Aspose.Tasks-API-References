---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie van objecten voor."
type: docs
weight: 321
url: /nl/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

Stelt een collectie van [TimephasedData](../../com.aspose.tasks/timephaseddata) objecten voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | Initialiseert een nieuw exemplaar van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | Voegt een [TimephasedData](../../com.aspose.tasks/timephaseddata) instantie toe aan dit collectieobject. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | Voegt een collectie van [TimephasedData](../../com.aspose.tasks/timephaseddata) instanties toe aan dit collectieobject. |
| [clear()](#clear--) | Verwijdert alle items uit de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | Bepaalt of de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) een specifieke waarde bevat. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | Kopieert de elementen van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) naar een Array, beginnend bij een specifieke Array-index. |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of de System.Collections.Generic.ICollection&lt;T&gt; alleen-lezen is. |
| [iterator()](#iterator--) | Retourneert een iterator voor deze collectie. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | Verwijdert een [TimephasedData](../../com.aspose.tasks/timephaseddata) instantie uit dit collectieobject. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | Selecteert alle tijdfasen tussen `startTime` en `finishTime`. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | Stelt het element in op de opgegeven index. |
| [size()](#size--) | Haalt het aantal objecten op dat in dit [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object zit. |
| [toList()](#toList--) | Converteert het [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object naar een lijst van [TimephasedData](../../com.aspose.tasks/timephaseddata) objecten. |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


Initialiseert een nieuw exemplaar van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse.

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


Voegt een [TimephasedData](../../com.aspose.tasks/timephaseddata) instantie toe aan dit collectieobject.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Het toe te voegen item. |

**Returns:**
boolean - true, als het item is toegevoegd; anders false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


Voegt een collectie van [TimephasedData](../../com.aspose.tasks/timephaseddata) instanties toe aan dit collectieobject.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | Een collectie van [TimephasedData](../../com.aspose.tasks/timephaseddata) objecten om toe te voegen. |

### clear() {#clear--}
```
public final void clear()
```


Verwijdert alle items uit de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


Bepaalt of de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) een specifieke waarde bevat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Het object om in de collectie te vinden. |

**Returns:**
boolean - true als `item` in de collectie wordt gevonden; anders false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


Kopieert de elementen van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) naar een Array, beginnend bij een specifieke Array-index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | De eendimensionale Array die de bestemming is van de elementen die gekopieerd zijn van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). De Array moet nulgebaseerde indexering hebben. |
| arrayIndex | int | De nulgebaseerde index in `array` waarop het kopiëren begint. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Haalt een waarde op die aangeeft of de System.Collections.Generic.ICollection&lt;T&gt; alleen-lezen is.

**Returns:**
boolean - true als de System.Collections.Generic.ICollection<T> alleen-lezen is; anders false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


Retourneert een iterator voor deze collectie.

**Returns:**
java.util.Iterator<com.aspose.tasks.TimephasedData> - een iterator voor deze collectie.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


Verwijdert een [TimephasedData](../../com.aspose.tasks/timephaseddata) instantie uit dit collectieobject.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Het item om te verwijderen. |

**Returns:**
boolean - true als `item` succesvol is verwijderd uit de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection); anders false. Deze methode geeft ook false terug als `item` niet wordt gevonden in de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


Selecteert alle tijdfasen tussen `startTime` en `finishTime`. Heeft O(log n) complexiteit in het gemiddelde geval.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| timephasedDataType | byte | Type van tijdfasen om te selecteren. |
| startTime | java.util.Date | Begin van het interval. |
| finishTime | java.util.Date | Einde van het interval. |

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - Retourneert een nieuw lijstobject van de gegevens van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) gesorteerd op de eigenschap Start.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


Stelt het element in op de opgegeven index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De nulgebaseerde index van het element dat moet worden ingesteld. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | het element om in te stellen. |

### size() {#size--}
```
public final int size()
```


Haalt het aantal objecten op dat in dit [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object zit.

**Returns:**
int - het aantal objecten dat in dit [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object zit.
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


Converteert het [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object naar een lijst van [TimephasedData](../../com.aspose.tasks/timephaseddata) objecten.

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - Lijst van [TimephasedData](../../com.aspose.tasks/timephaseddata) objecten.
