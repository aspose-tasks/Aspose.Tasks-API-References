---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie voor die objecten bevat."
type: docs
weight: 234
url: /nl/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Stelt een collectie voor die [Rate](../../com.aspose.tasks/rate) objecten bevat.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Voegt een nieuw [Rate](../../com.aspose.tasks/rate) exemplaar toe aan deze collectie. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Voegt een nieuw [Rate](../../com.aspose.tasks/rate) exemplaar toe aan deze collectie. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\\} |
| [getByRateType(int key)](#getByRateType-int-) | Retourneert het element op de opgegeven index. |
| [getParentResource()](#getParentResource--) | Haalt het bovenliggende [Resource](../../com.aspose.tasks/resource) object op voor deze collectie. |
| [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is. |
| [iterator()](#iterator--) | Retourneert een enumerator voor deze collectie. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Verwijdert Rate-instantie uit deze collectie. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Stelt het element in op de opgegeven index. |
| [size()](#size--) | Haalt het aantal elementen op dat in de RateCollection zit. |
| [toList()](#toList--) | Converteert het [RateCollection](../../com.aspose.tasks/ratecollection) object naar een lijst van [Rate](../../com.aspose.tasks/rate) objecten. |
| [toList(int type)](#toList-int-) | Converteert het [RateCollection](../../com.aspose.tasks/ratecollection) object naar een lijst van [Rate](../../com.aspose.tasks/rate) objecten gefilterd op het opgegeven [RateType](../../com.aspose.tasks/ratetype) type. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Voegt een nieuw [Rate](../../com.aspose.tasks/rate) exemplaar toe aan deze collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| ratesFrom | java.util.Date | De datum waarop het nieuwe tarief van kracht wordt. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Voegt een nieuw [Rate](../../com.aspose.tasks/rate) exemplaar toe aan deze collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| ratesFrom | java.util.Date | De datum waarop het nieuwe tarief van kracht wordt. |
| type | int | De tarieftabel waarin moet worden toegevoegd. |

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


(@inheritDoc\\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\\}

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Retourneert het element op de opgegeven index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | int | De nulgebaseerde index van het element om op te halen. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Haalt het bovenliggende [Resource](../../com.aspose.tasks/resource) object op voor deze collectie.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Haalt een waarde op die aangeeft of deze collectie alleen-lezen is.

**Returns:**
boolean - een waarde die aangeeft of deze collectie alleen-lezen is.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Retourneert een enumerator voor deze collectie.

**Returns:**
java.util.Iterator - een enumerator voor deze collectie.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\\}

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Verwijdert Rate-instantie uit deze collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | Het item om te verwijderen. |

**Returns:**
boolean - true als de opgegeven Rate succesvol is verwijderd; anders false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Stelt het element in op de opgegeven index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | int | De nulgebaseerde index van het element dat moet worden ingesteld. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | Het element dat moet worden ingesteld op de opgegeven index. |

### size() {#size--}
```
public final int size()
```


Haalt het aantal elementen op dat in de RateCollection zit.

**Returns:**
int - het aantal elementen dat zich bevindt in de RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Converteert het [RateCollection](../../com.aspose.tasks/ratecollection) object naar een lijst van [Rate](../../com.aspose.tasks/rate) objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Lijst van [Rate](../../com.aspose.tasks/rate) objecten.
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Converteert het [RateCollection](../../com.aspose.tasks/ratecollection) object naar een lijst van [Rate](../../com.aspose.tasks/rate) objecten gefilterd op het opgegeven [RateType](../../com.aspose.tasks/ratetype) type.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| type | int | Het type om op te filteren. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - een lijst van [Rate](../../com.aspose.tasks/rate) objecten.
