---
title: TimephasedDataCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection of  objects.
type: docs
weight: 320
url: /java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

Represents a collection of [TimephasedData](../../com.aspose.tasks/timephaseddata) objects.
## Constructors

| Constructor | Description |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | Initializes a new instance of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class. |
## Methods

| Method | Description |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | Adds [TimephasedData](../../com.aspose.tasks/timephaseddata) instance to this collection object. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | Adds a collection of [TimephasedData](../../com.aspose.tasks/timephaseddata) instances to this collection object. |
| [clear()](#clear--) | Removes all items from the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | Determines whether the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contains a specific value. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | Copies the elements of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) to an Array, starting at a particular Array index. |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether the System.Collections.Generic.ICollection&lt;T&gt; is read-only. |
| [iterator()](#iterator--) | Returns an iterator for this collection. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | Removes [TimephasedData](../../com.aspose.tasks/timephaseddata) instance from this collection object. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | Selects all time phases between `startTime` and `finishTime`. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | Sets the element at the specified index. |
| [size()](#size--) | Gets the number of objects contained in this [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object. |
| [toList()](#toList--) | Converts the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object to a list of [TimephasedData](../../com.aspose.tasks/timephaseddata) objects. |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


Initializes a new instance of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class.

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


Adds [TimephasedData](../../com.aspose.tasks/timephaseddata) instance to this collection object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | The item to add. |

**Returns:**
boolean - true, if item was added; otherwise false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


Adds a collection of [TimephasedData](../../com.aspose.tasks/timephaseddata) instances to this collection object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | A collection of [TimephasedData](../../com.aspose.tasks/timephaseddata) objects to add. |

### clear() {#clear--}
```
public final void clear()
```


Removes all items from the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


Determines whether the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contains a specific value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | The object to locate in the collection. |

**Returns:**
boolean - true if `item` is found in the collection; otherwise, false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


Copies the elements of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) to an Array, starting at a particular Array index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | The one-dimensional Array that is the destination of the elements copied from [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). The Array must have zero-based indexing. |
| arrayIndex | int | The zero-based index in `array` at which copying begins. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Gets a value indicating whether the System.Collections.Generic.ICollection&lt;T&gt; is read-only.

**Returns:**
boolean - true if the System.Collections.Generic.ICollection&lt;T&gt; is read-only; otherwise, false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


Returns an iterator for this collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.TimephasedData&gt; - an iterator for this collection.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


Removes [TimephasedData](../../com.aspose.tasks/timephaseddata) instance from this collection object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | The item to remove. |

**Returns:**
boolean - true if `item` was successfully removed from the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection); otherwise, false. This method also returns false if `item` is not found in the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


Selects all time phases between `startTime` and `finishTime`. Has O(log n) complexity in average case.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| timephasedDataType | byte | Type of time phases to select. |
| startTime | java.util.Date | Interval's start. |
| finishTime | java.util.Date | Interval's finish. |

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Returns new list instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) data ordered by Start property.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


Sets the element at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the element to set. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | the element to set. |

### size() {#size--}
```
public final int size()
```


Gets the number of objects contained in this [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object.

**Returns:**
int - the number of objects contained in this [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object.
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


Converts the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object to a list of [TimephasedData](../../com.aspose.tasks/timephaseddata) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - List of [TimephasedData](../../com.aspose.tasks/timephaseddata) objects.
