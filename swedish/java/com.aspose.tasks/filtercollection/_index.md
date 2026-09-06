---
title: "FilterCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Innehåller en lista med  objekt."
type: docs
weight: 92
url: /sv/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

Innehåller en lista med [Filter](../../com.aspose.tasks/filter)-objekt. Implementerar ICollection&lt;Filter&gt;-gränssnittet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | Tar bort alla element från denna samling (valfri operation). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | Returnerar true om denna samling innehåller det angivna objektet. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | Kopierar elementen från den angivna arrayen till denna samling med start från det angivna indexet. |
| [iterator()](#iterator--) | Returnerar en iterator över elementen som finns i denna samling. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | Tar bort det angivna objektet från denna samling. |
| [size()](#size--) | Hämtar antalet element som finns i denna samling. |
| [toList()](#toList--) | Konverterar en filtersamling till en lista med `Filter`-objekt. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


Tar bort alla element från denna samling (valfri operation).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


Returnerar true om denna samling innehåller det angivna objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | det angivna objektet. |

**Returns:**
boolean - true om samlingen innehåller det angivna objektet.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


Kopierar elementen från den angivna arrayen till denna samling med start från det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | den angivna endimensionella arrayen att kopiera element till |
| arrayIndex | int | det nollbaserade indexet för den angivna arrayen där kopieringen börjar. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


Returnerar en iterator över elementen som finns i denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - samlingsiterator.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


Tar bort det angivna objektet från denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | det angivna objektet. |

**Returns:**
boolean - true om operationen lyckades.
### size() {#size--}
```
public final int size()
```


Hämtar antalet element som finns i denna samling.

**Returns:**
int - antalet element som finns i denna samling.
### toList() {#toList--}
```
public List<Filter> toList()
```


Konverterar en filtersamling till en lista med `Filter`-objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - generisk lista med `Filter`-objekt.
