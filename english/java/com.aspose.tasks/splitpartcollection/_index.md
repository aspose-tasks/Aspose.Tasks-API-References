---
title: SplitPartCollection
second_title: Aspose.Tasks for Java API Reference
description: Collection that represents the portions of a task.
type: docs
weight: 278
url: /java/com.aspose.tasks/splitpartcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class SplitPartCollection extends AbstractList<SplitPart>
```

Collection that represents the portions of a task.
## Methods

| Method | Description |
| --- | --- |
| [get(int index)](#get-int-) | Retrieves a task's split part at the given index. |
| [set(int index, SplitPart value)](#set-int-com.aspose.tasks.SplitPart-) | Sets a task's split part at the given index. |
| [size()](#size--) | Gets the number of parts in the collection. |
| [toArray()](#toArray--) | Copies all parts from the collection to a new array. |
### get(int index) {#get-int-}
```
public final SplitPart get(int index)
```


Retrieves a task's split part at the given index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The part index.

--------------------

The index is zero-based. Returns null if the index is outside array's boundaries. |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### set(int index, SplitPart value) {#set-int-com.aspose.tasks.SplitPart-}
```
public final SplitPart set(int index, SplitPart value)
```


Sets a task's split part at the given index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The part index.

--------------------

The index is zero-based. Returns null if the index is outside array's boundaries. |
| value | [SplitPart](../../com.aspose.tasks/splitpart) | a split part to set. |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### size() {#size--}
```
public final int size()
```


Gets the number of parts in the collection.

**Returns:**
int - the number of parts in the collection.
### toArray() {#toArray--}
```
public final SplitPart[] toArray()
```


Copies all parts from the collection to a new array.

**Returns:**
com.aspose.tasks.SplitPart[] - An array of [SplitPart](../../com.aspose.tasks/splitpart) objects.
