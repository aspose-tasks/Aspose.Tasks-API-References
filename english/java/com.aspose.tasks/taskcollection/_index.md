---
title: TaskCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection of  objects.
type: docs
weight: 292
url: /java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Represents a collection of [Task](../../com.aspose.tasks/task) objects.
## Methods

| Method | Description |
| --- | --- |
| [add()](#add--) | Adds new task to project tasks collection on the same outline level of the last task. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Inserts a new task before a task with the specified id and on the same outline level. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Add the specified task to the instance of the [TaskCollection](../../com.aspose.tasks/taskcollection) class. |
| [add(String taskName)](#add-java.lang.String-) | Adds a new task to children tasks collection. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Adds a new recurring task to children tasks collection. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Checks if collection contains specified item. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Returns a task with the specified Id whose ancestor is parent task of this collection . |
| [getByUid(int uid)](#getByUid-int-) | Returns a task with the specified Uid whose ancestor is parent task of this collection . |
| [getParentProject()](#getParentProject--) | Gets the parent project of the TaskCollection object. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether this collection is read only. |
| [iterator()](#iterator--) | Returns an enumerator for this collection. |
| [remove(Object item)](#remove-java.lang.Object-) | This is the stub implementation of ICollection's Remove method, that only throws UnsupportedOperationException |
| [size()](#size--) | Gets the number of objects contained in the TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converts the TaskCollection object to a list of [Task](../../com.aspose.tasks/task) objects. |
### add() {#add--}
```
public final Task add()
```


Adds new task to project tasks collection on the same outline level of the last task.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Inserts a new task before a task with the specified id and on the same outline level.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | The parameters the specified parameters for creation of recurring task. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Add the specified task to the instance of the [TaskCollection](../../com.aspose.tasks/taskcollection) class. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, ids and outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | the specified task which should be added to this task collection. |

**Returns:**
boolean - true if operation was successful.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Adds a new task to children tasks collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskName | java.lang.String | the specified task name. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Adds a new recurring task to children tasks collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskName | java.lang.String | the specified task name. |
| beforeTaskId | int | The specified id of a task before which a new task will be inserted. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


Checks if collection contains specified item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | The item to check. |

**Returns:**
boolean - true, if collection contains an item, false otherwise.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Returns a task with the specified Id whose ancestor is parent task of this collection .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Returns a task with the specified Uid whose ancestor is parent task of this collection .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project of the TaskCollection object.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
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
public final Iterator<Task> iterator()
```


Returns an enumerator for this collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - an enumerator for this collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


This is the stub implementation of ICollection's Remove method, that only throws UnsupportedOperationException

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | java.lang.Object | The item to remove. |

**Returns:**
boolean - `true` if the item was removed; `false` otherwise.
### size() {#size--}
```
public final int size()
```


Gets the number of objects contained in the TaskCollection.

**Returns:**
int - the number of objects contained in the TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Converts the TaskCollection object to a list of [Task](../../com.aspose.tasks/task) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - returns a list which contains the [Task](../../com.aspose.tasks/task) class instances of this collection.
