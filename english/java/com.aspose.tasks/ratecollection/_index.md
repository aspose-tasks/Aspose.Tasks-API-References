---
title: RateCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection which contains  objects.
type: docs
weight: 233
url: /java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Represents a collection which contains [Rate](../../com.aspose.tasks/rate) objects.
## Methods

| Method | Description |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Adds a new [Rate](../../com.aspose.tasks/rate) instance to this collection. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Adds a new [Rate](../../com.aspose.tasks/rate) instance to this collection. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Returns the element at the specified index. |
| [getParentResource()](#getParentResource--) | Gets the parent [Resource](../../com.aspose.tasks/resource) object for this collection. |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether this collection is read only. |
| [iterator()](#iterator--) | Returns an enumerator for this collection. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Removes Rate instance from this collection. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Sets the element at the specified index. |
| [size()](#size--) | Gets the number of elements contained in the RateCollection. |
| [toList()](#toList--) | Converts the [RateCollection](../../com.aspose.tasks/ratecollection) object to a list of [Rate](../../com.aspose.tasks/rate) objects. |
| [toList(int type)](#toList-int-) | Converts the [RateCollection](../../com.aspose.tasks/ratecollection) object to a list of [Rate](../../com.aspose.tasks/rate) objects filtered by specified [RateType](../../com.aspose.tasks/ratetype) type. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Adds a new [Rate](../../com.aspose.tasks/rate) instance to this collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ratesFrom | java.util.Date | The date the new rate comes into effect. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Adds a new [Rate](../../com.aspose.tasks/rate) instance to this collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ratesFrom | java.util.Date | The date the new rate comes into effect. |
| type | int | The rate table to add into. |

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
| Parameter | Type | Description |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Returns the element at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The zero-based index of the element to get. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Gets the parent [Resource](../../com.aspose.tasks/resource) object for this collection.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Gets a value indicating whether this collection is read only.

**Returns:**
boolean - a value indicating whether this collection is read only.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Returns an enumerator for this collection.

**Returns:**
java.util.Iterator - an enumerator for this collection.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Removes Rate instance from this collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | The item to remove. |

**Returns:**
boolean - true if the specified Rate was removed successfully; otherwise, false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Sets the element at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The zero-based index of the element to set. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | The element to set at the specified index. |

### size() {#size--}
```
public final int size()
```


Gets the number of elements contained in the RateCollection.

**Returns:**
int - the number of elements contained in the RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Converts the [RateCollection](../../com.aspose.tasks/ratecollection) object to a list of [Rate](../../com.aspose.tasks/rate) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - List of [Rate](../../com.aspose.tasks/rate) objects.
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Converts the [RateCollection](../../com.aspose.tasks/ratecollection) object to a list of [Rate](../../com.aspose.tasks/rate) objects filtered by specified [RateType](../../com.aspose.tasks/ratetype) type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | The type to filter on. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - a list of [Rate](../../com.aspose.tasks/rate) objects.
