---
title: ReadOnlyCollectionBase
second_title: Aspose.Tasks for Java API Reference
description: Represents a read-only collection of objects.
type: docs
weight: 237
url: /java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Represents a read-only collection of objects.

 T : Type of collection items.
## Methods

| Method | Description |
| --- | --- |
| [add(T item)](#add-T-) | This is the stub implementation of ICollection's Add method, that only throws UnsupportedOperationException |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Returns the element at the specified index. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Determines, if collection read-only. |
| [iterator()](#iterator--) | Returns an enumerator for this collection. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Returns the element at the specified index. |
| [size()](#size--) | Gets the number of objects contained in the object. |
| [toList()](#toList--) | Converts the collection to a list of objects. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


This is the stub implementation of ICollection's Add method, that only throws UnsupportedOperationException

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | T | The item to add. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Returns the element at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the element to get. |

**Returns:**
T - the element at the specified index.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Determines, if collection read-only.

**Returns:**
boolean - true if collection read-only; false otherwise.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Returns an enumerator for this collection.

**Returns:**
java.util.Iterator&lt;T&gt; - An enumerator for this collection.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
T - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Returns the element at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the element to get. |
| value | T |  |

**Returns:**
T - the element at the specified index.
### size() {#size--}
```
public final int size()
```


Gets the number of objects contained in the object.

**Returns:**
int - the number of objects contained in the object.
### toList() {#toList--}
```
public final List<T> toList()
```


Converts the collection to a list of objects.

**Returns:**
java.util.List&lt;T&gt; - Generic list of objects.
