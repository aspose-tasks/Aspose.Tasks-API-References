---
title: "FilterCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Bevat een lijst van objecten."
type: docs
weight: 92
url: /nl/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

Bevat een lijst van [Filter](../../com.aspose.tasks/filter)-objecten. Implementeert de ICollection&lt;Filter&gt;-interface.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | Verwijdert alle elementen uit deze collectie (optionele bewerking). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | Retourneert true als deze collectie het opgegeven item bevat. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | Kopieert de elementen van de opgegeven array naar deze collectie, beginnend bij de opgegeven index. |
| [iterator()](#iterator--) | Retourneert een iterator over de elementen die zich in deze collectie bevinden. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | Verwijdert het opgegeven item uit deze collectie. |
| [size()](#size--) | Haalt het aantal elementen op dat in deze collectie zit. |
| [toList()](#toList--) | Converteert een filtercollectie naar een lijst van `Filter` objecten. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


Verwijdert alle elementen uit deze collectie (optionele bewerking).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


Retourneert true als deze collectie het opgegeven item bevat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | het opgegeven item. |

**Returns:**
boolean - true als de collectie het opgegeven item bevat.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


Kopieert de elementen van de opgegeven array naar deze collectie, beginnend bij de opgegeven index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | de opgegeven één-dimensionale array om elementen naar te kopiëren |
| arrayIndex | int | de nulgebaseerde index van de opgegeven array waarop het kopiëren begint. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


Retourneert een iterator over de elementen die zich in deze collectie bevinden.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - collectie-iterator.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


Verwijdert het opgegeven item uit deze collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | het opgegeven item. |

**Returns:**
boolean - true als de bewerking succesvol was.
### size() {#size--}
```
public final int size()
```


Haalt het aantal elementen op dat in deze collectie zit.

**Returns:**
int - het aantal elementen dat in deze collectie zit.
### toList() {#toList--}
```
public List<Filter> toList()
```


Converteert een filtercollectie naar een lijst van `Filter` objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - generieke lijst van `Filter` objecten.
