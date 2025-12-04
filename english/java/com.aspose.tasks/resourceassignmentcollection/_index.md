---
title: ResourceAssignmentCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection of  objects.
type: docs
weight: 249
url: /java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Represents a collection of [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objects.
## Methods

| Method | Description |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | This is the stub implementation of ICollection's Add method, that only throws UnsupportedOperationException |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Adds new assignment to the ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Adds new assignment to the ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Adds new assignment to the ResourceAssignmentCollection. |
| [clear()](#clear--) | Removes all items from the collection. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Returns an assignment with the specified uid. |
| [getParentProject()](#getParentProject--) | Gets the parent project of the ResourceAssignmentCollection object. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether this collection is read only. |
| [iterator()](#iterator--) | Returns an enumerator for this collection. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Removes specified assignment from collection, if it is not read-only, otherwise throws UnsupportedOperationException. |
| [size()](#size--) | Gets the number of objects contained in the ResourceAssignmentCollection. |
| [toList()](#toList--) | Converts the ResourceAssignmentCollection object to a list of [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objects. |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


This is the stub implementation of ICollection's Add method, that only throws UnsupportedOperationException

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | The item to remove. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Adds new assignment to the ResourceAssignmentCollection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | A task to be assigned. |
| resource | [Resource](../../com.aspose.tasks/resource) | A resource to be assigned. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Adds new assignment to the ResourceAssignmentCollection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | A task to be assigned. |
| resource | [Resource](../../com.aspose.tasks/resource) | A resource to be assigned. |
| units | double | The number of units for a new assignment. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Adds new assignment to the ResourceAssignmentCollection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | A task to be assigned. |
| resource | [Resource](../../com.aspose.tasks/resource) | A cost resource to be assigned. |
| cost | java.math.BigDecimal | The cost for a new assignment. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Removes all items from the collection.

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Returns an assignment with the specified uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | The specified uid.

--------------------

O(1) complexity. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project of the ResourceAssignmentCollection object.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


Gets a value indicating whether this collection is read only.

**Returns:**
boolean - a value indicating whether this collection is read only.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Returns an enumerator for this collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - an enumerator for this collection.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Removes specified assignment from collection, if it is not read-only, otherwise throws UnsupportedOperationException.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The assignment to remove. |

**Returns:**
boolean - true, if specified item was removed, false otherwise.
### size() {#size--}
```
public final int size()
```


Gets the number of objects contained in the ResourceAssignmentCollection.

**Returns:**
int - the number of objects contained in the ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Converts the ResourceAssignmentCollection object to a list of [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - List of [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objects.
