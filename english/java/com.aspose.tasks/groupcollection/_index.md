---
title: GroupCollection
second_title: Aspose.Tasks for Java API Reference
description: Contains a list of  objects.
type: docs
weight: 117
url: /java/com.aspose.tasks/groupcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class GroupCollection extends AbstractCollection<Group>
```

Contains a list of [Group](../../com.aspose.tasks/group) objects. Implements ICollection&lt;Group&gt; interface.
## Methods

| Method | Description |
| --- | --- |
| [add(Group item)](#add-com.aspose.tasks.Group-) |  |
| [clear()](#clear--) |  |
| [contains(Group item)](#contains-com.aspose.tasks.Group-) | Returns true if this collection contains the specified item. |
| [copyTo(Group[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Group---int-) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [getParentProject()](#getParentProject--) | Gets the parent of the Group object. |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether this collection is read-only. |
| [iterator()](#iterator--) |  |
| [remove(Group item)](#remove-com.aspose.tasks.Group-) | Removes the first occurrence of a specific object from this collection. |
| [size()](#size--) | Gets the number of elements contained in this collection. |
| [toList()](#toList--) | Converts a group collection to a list of [Group](../../com.aspose.tasks/group) objects. |
### add(Group item) {#add-com.aspose.tasks.Group-}
```
public final boolean add(Group item)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Group](../../com.aspose.tasks/group) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public final void clear()
```




### contains(Group item) {#contains-com.aspose.tasks.Group-}
```
public final boolean contains(Group item)
```


Returns true if this collection contains the specified item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Group](../../com.aspose.tasks/group) | the specified item. |

**Returns:**
boolean - true if the collection contains the specified item.
### copyTo(Group[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Group---int-}
```
public final void copyTo(Group[] array, int arrayIndex)
```


Copies the elements of this collection to the specified array, starting at the specified array index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | [Group\[\]](../../com.aspose.tasks/group) | the specified one-dimensional array to copy elements to |
| arrayIndex | int | the zero-based index of the specified array at which copying begins. |

### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent of the Group object. Read-only [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the Group object.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Gets a value indicating whether this collection is read-only.

**Returns:**
boolean - a value indicating whether this collection is read-only.
### iterator() {#iterator--}
```
public Iterator<Group> iterator()
```




**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Group&gt;
### remove(Group item) {#remove-com.aspose.tasks.Group-}
```
public final boolean remove(Group item)
```


Removes the first occurrence of a specific object from this collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Group](../../com.aspose.tasks/group) | the specified object to remove. |

**Returns:**
boolean - true if the specified object was successfully removed from this collection; otherwise, false.
### size() {#size--}
```
public final int size()
```


Gets the number of elements contained in this collection.

**Returns:**
int - the number of elements contained in this collection.
### toList() {#toList--}
```
public final List<Group> toList()
```


Converts a group collection to a list of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.Group&gt; - Generic list of [Group](../../com.aspose.tasks/group) objects.
