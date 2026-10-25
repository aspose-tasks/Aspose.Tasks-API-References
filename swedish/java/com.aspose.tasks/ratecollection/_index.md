---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling som innehåller objekt."
type: docs
weight: 234
url: /sv/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Representerar en samling som innehåller [Rate](../../com.aspose.tasks/rate) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Lägger till en ny [Rate](../../com.aspose.tasks/rate) instans i denna samling. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Lägger till en ny [Rate](../../com.aspose.tasks/rate) instans i denna samling. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Returnerar elementet på det angivna indexet. |
| [getParentResource()](#getParentResource--) | Hämtar det överordnade [Resource](../../com.aspose.tasks/resource) objektet för denna samling. |
| [isReadOnly()](#isReadOnly--) | Hämtar ett värde som indikerar om denna samling är skrivskyddad. |
| [iterator()](#iterator--) | Returnerar en enumerator för denna samling. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Tar bort Rate-instans från denna samling. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Ställer in elementet på det angivna indexet. |
| [size()](#size--) | Hämtar antalet element som finns i RateCollection. |
| [toList()](#toList--) | Konverterar [RateCollection](../../com.aspose.tasks/ratecollection)-objektet till en lista med [Rate](../../com.aspose.tasks/rate)-objekt. |
| [toList(int type)](#toList-int-) | Konverterar [RateCollection](../../com.aspose.tasks/ratecollection)-objektet till en lista med [Rate](../../com.aspose.tasks/rate)-objekt filtrerade efter angiven [RateType](../../com.aspose.tasks/ratetype)-typ. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Lägger till en ny [Rate](../../com.aspose.tasks/rate) instans i denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ratesFrom | java.util.Date | Datumet då den nya räntan träder i kraft. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Lägger till en ny [Rate](../../com.aspose.tasks/rate) instans i denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ratesFrom | java.util.Date | Datumet då den nya räntan träder i kraft. |
| typ | int | Räntetabellen att lägga till i. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Returnerar elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | int | Det nollbaserade indexet för elementet att hämta. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Hämtar det överordnade [Resource](../../com.aspose.tasks/resource) objektet för denna samling.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Hämtar ett värde som indikerar om denna samling är skrivskyddad.

**Returns:**
boolean - ett värde som indikerar om denna samling är skrivskyddad.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Returnerar en enumerator för denna samling.

**Returns:**
java.util.Iterator - en enumerator för denna samling.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Tar bort Rate-instans från denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | Objektet som ska tas bort. |

**Returns:**
boolean - true om den angivna Rate togs bort framgångsrikt; annars false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Ställer in elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | int | Det nollbaserade indexet för elementet som ska sättas. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | Elementet som ska sättas på det angivna indexet. |

### size() {#size--}
```
public final int size()
```


Hämtar antalet element som finns i RateCollection.

**Returns:**
int - antalet element som finns i RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Konverterar [RateCollection](../../com.aspose.tasks/ratecollection)-objektet till en lista med [Rate](../../com.aspose.tasks/rate)-objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Lista med [Rate](../../com.aspose.tasks/rate) objekt.
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Konverterar [RateCollection](../../com.aspose.tasks/ratecollection)-objektet till en lista med [Rate](../../com.aspose.tasks/rate)-objekt filtrerade efter angiven [RateType](../../com.aspose.tasks/ratetype)-typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | int | Typen att filtrera på. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - en lista med [Rate](../../com.aspose.tasks/rate) objekt.
