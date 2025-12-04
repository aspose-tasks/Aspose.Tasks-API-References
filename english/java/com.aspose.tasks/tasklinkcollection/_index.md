---
title: TaskLinkCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection of  objects.
type: docs
weight: 295
url: /java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Represents a collection of [Task](../../com.aspose.tasks/task) objects.
## Methods

| Method | Description |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Returns an instance of Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) which has been added to the TaskLinkCollection object. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Returns an instance of [TaskLink](../../com.aspose.tasks/tasklink) which has been added to the TaskLinkCollection object. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Returns an instance of [TaskLink](../../com.aspose.tasks/tasklink) which has been added to the TaskLinkCollection object. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | This is the stub implementation of ICollection's Add method, that only throws UnsupportedOperationException |
| [clear()](#clear--) | Reserved for internal usage. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Gets the parent project of the ResourceAssignmentCollection object. |
| [remove(int index)](#remove-int-) | Removes the element at the specified position in this collection and returns the element that was removed from the collection. |
| [remove(Object item)](#remove-java.lang.Object-) | Removes task link from a project. |
| [size()](#size--) | Returns the number of objects contained in this `TaskLinkCollection` object. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converts the TaskLinkCollection object to a list of [TaskLink](../../com.aspose.tasks/tasklink) objects. |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Returns an instance of Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) which has been added to the TaskLinkCollection object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Predecessor task. |
| succ | [Task](../../com.aspose.tasks/task) | Successor task. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Returns an instance of [TaskLink](../../com.aspose.tasks/tasklink) which has been added to the TaskLinkCollection object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Predecessor task. |
| succ | [Task](../../com.aspose.tasks/task) | Successor task. |
| linkType | int | Link type [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Returns an instance of [TaskLink](../../com.aspose.tasks/tasklink) which has been added to the TaskLinkCollection object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Predecessor task. |
| succ | [Task](../../com.aspose.tasks/task) | Successor task. |
| linkType | int | Link type [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Link lag [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


This is the stub implementation of ICollection's Add method, that only throws UnsupportedOperationException

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | The item to add. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Reserved for internal usage.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project of the ResourceAssignmentCollection object.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Removes the element at the specified position in this collection and returns the element that was removed from the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the specified position to remove the element at. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Removes task link from a project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | java.lang.Object | the specified instance of `TaskLink` class to remove. |

**Returns:**
boolean - returns the instance of `TaskLink` class which was removed from this collection.
### size() {#size--}
```
public final int size()
```


Returns the number of objects contained in this `TaskLinkCollection` object. Read only `int`.

**Returns:**
int - returns the number of objects contained in this collection.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Converts the TaskLinkCollection object to a list of [TaskLink](../../com.aspose.tasks/tasklink) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - List of [TaskLink](../../com.aspose.tasks/tasklink) objects.
