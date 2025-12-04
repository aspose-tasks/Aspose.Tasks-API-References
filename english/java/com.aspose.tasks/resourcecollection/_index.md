---
title: ResourceCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection of  objects.
type: docs
weight: 250
url: /java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Represents a collection of [Resource](../../com.aspose.tasks/resource) objects.
## Methods

| Method | Description |
| --- | --- |
| [add()](#add--) | Adds new resource at the last position of a project resources collection. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Adds new resource at the last position of a project resources collection. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Adds new resource at the specified position of a project resources collection. |
| [clear()](#clear--) | Direct clearing is not supported, this method just throw UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Returns a resource with the specified id. |
| [getByUid(int uid)](#getByUid-int-) | Returns a resource with the specified Uid. |
| [getParentProject()](#getParentProject--) | Gets the parent project of the ResourceCollection object. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Returns an enumerator for this collection. |
| [remove(Object o)](#remove-java.lang.Object-) | This is the stub implementation of Collection's remove method, that only throws UnsupportedOperationException |
| [size()](#size--) | Gets the number of elements contained in the ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converts the ResourceCollection object to a list of [Resource](../../com.aspose.tasks/resource) objects. |
### add() {#add--}
```
public final Resource add()
```


Adds new resource at the last position of a project resources collection.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Adds new resource at the last position of a project resources collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| resourceName | java.lang.String | Name of a resource. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Adds new resource at the specified position of a project resources collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| resourceName | java.lang.String | Name of a resource. |
| beforeResourceId | int | Position of the previous resource in a project resources collection. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Direct clearing is not supported, this method just throw UnsupportedOperationException.

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
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Returns a resource with the specified id.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | int | The specified id.

--------------------

O(1) complexity. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Returns a resource with the specified Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | The specified uid.

--------------------

O(1) complexity. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project of the ResourceCollection object.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Returns an enumerator for this collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - an enumerator for this collection.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


This is the stub implementation of Collection's remove method, that only throws UnsupportedOperationException

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | the item to remove. |

**Returns:**
boolean - `true` if the item was removed; `false` otherwise.
### size() {#size--}
```
public final int size()
```


Gets the number of elements contained in the ResourceCollection.

--------------------

Read-only `int`.

**Returns:**
int - the number of elements contained in the ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Converts the ResourceCollection object to a list of [Resource](../../com.aspose.tasks/resource) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - List of [Resource](../../com.aspose.tasks/resource) objects.
