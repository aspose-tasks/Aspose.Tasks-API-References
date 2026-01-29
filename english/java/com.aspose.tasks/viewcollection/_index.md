---
title: ViewCollection
second_title: Aspose.Tasks for Java API Reference
description: Contains a list of  objects.
type: docs
weight: 342
url: /java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Contains a list of [View](../../com.aspose.tasks/view) objects. Extends `AbstractCollection` class.
## Methods

| Method | Description |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Adds the specified item to this collection. |
| [clear()](#clear--) | Removes all items from this collection. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Returns true if the specified item is found in this collection; otherwise, false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Searches for a View with the name, and returns the first occurrence within the collection. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Searches for a View with the specified Screen property, and returns the first occurrence within the collection. |
| [getParentProject()](#getParentProject--) | Gets the parent of the View object. |
| [iterator()](#iterator--) | Returns an iterator over the elements contained in this collection. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Removes the first occurrence of a specific object from this collection. |
| [size()](#size--) | Gets the number of elements contained in this collection. |
| [toList()](#toList--) | Converts a view collection to a list of [View](../../com.aspose.tasks/view) objects. |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Adds the specified item to this collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | the specified item to add to this collection. |

**Returns:**
boolean - true if the operation was successful.
### clear() {#clear--}
```
public final void clear()
```


Removes all items from this collection.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Returns true if the specified item is found in this collection; otherwise, false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | the specified item to find. |

**Returns:**
boolean - true if the specified item is found in this collection; otherwise, false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Copies the elements of this collection to the specified array, starting at the specified array index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | the specified one-dimensional array to copy elements to |
| arrayIndex | int | the zero-based index of the specified array at which copying begins. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Searches for a View with the name, and returns the first occurrence within the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| viewName | java.lang.String | Name of the View to search. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Searches for a View with the specified Screen property, and returns the first occurrence within the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) enumeration value. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent of the View object. Read-only [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Returns an iterator over the elements contained in this collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - collection iterator.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Removes the first occurrence of a specific object from this collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | the specified object to remove. |

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
public final List<View> toList()
```


Converts a view collection to a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Generic list of [View](../../com.aspose.tasks/view) objects.
