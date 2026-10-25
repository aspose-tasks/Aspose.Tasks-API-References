---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 293
url: /zh/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

表示一个 [Task](../../com.aspose.tasks/task) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add()](#add--) | 在与最后一个任务相同的大纲级别上向项目任务集合添加新任务。 |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | 在具有指定 ID 的任务之前插入新任务，并保持相同的大纲级别。 |
| [add(Task item)](#add-com.aspose.tasks.Task-) | 将指定任务添加到 [TaskCollection](../../com.aspose.tasks/taskcollection) 类的实例中。 |
| [add(String taskName)](#add-java.lang.String-) | 向子任务集合添加新任务。 |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | 向子任务集合添加新的循环任务。 |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | 检查集合是否包含指定的项。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | 返回具有指定 Id 且其祖先是此集合的父任务的任务。 |
| [getByUid(int uid)](#getByUid-int-) | 返回具有指定 Uid 且其祖先是此集合的父任务的任务。 |
| [getParentProject()](#getParentProject--) | 获取 TaskCollection 对象的父项目。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 获取指示此集合是否只读的值。 |
| [iterator()](#iterator--) | 返回此集合的枚举器。 |
| [remove(Object item)](#remove-java.lang.Object-) | 这是 ICollection 的 Remove 方法的存根实现，只会抛出 UnsupportedOperationException。 |
| [size()](#size--) | 获取 TaskCollection 中包含的对象数量。 |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | 将 TaskCollection 对象转换为 [Task](../../com.aspose.tasks/task) 对象的列表。 |
### add() {#add--}
```
public final Task add()
```


在与最后一个任务相同的大纲级别上向项目任务集合添加新任务。

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


在具有指定 ID 的任务之前插入新任务，并保持相同的大纲级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | 用于创建循环任务的指定参数。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


将指定任务添加到 [TaskCollection](../../com.aspose.tasks/taskcollection) 类的实例中。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置提前/延后日期）并计算诸如时差、工作和成本字段、ID 和大纲级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 ID、大纲级别和大纲编号。如果 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务（开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段，重新计算 ID 和大纲级别）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | 应添加到此任务集合的指定任务。 |

**Returns:**
boolean - 如果操作成功则为 true。
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


向子任务集合添加新任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| taskName | java.lang.String | 指定的任务名称。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


向子任务集合添加新的循环任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| taskName | java.lang.String | 指定的任务名称。 |
| beforeTaskId | int | 在其前插入新任务的任务的指定 ID。 |

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


检查集合是否包含指定的项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | 要检查的项。 |

**Returns:**
boolean - 如果集合包含项则为 true，否则为 false。
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


返回具有指定 Id 且其祖先是此集合的父任务的任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


返回具有指定 Uid 且其祖先是此集合的父任务的任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取 TaskCollection 对象的父项目。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


获取指示此集合是否只读的值。

**Returns:**
boolean - 指示此集合是否只读的值。
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


返回此集合的枚举器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - 此集合的枚举器。
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


这是 ICollection 的 Remove 方法的存根实现，只会抛出 UnsupportedOperationException。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | java.lang.Object | 要删除的项目。 |

**Returns:**
boolean - 如果该项已被移除，则为 `true`；否则为 `false`。
### size() {#size--}
```
public final int size()
```


获取 TaskCollection 中包含的对象数量。

**Returns:**
int - TaskCollection 中包含的对象数量。
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


将 TaskCollection 对象转换为 [Task](../../com.aspose.tasks/task) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - 返回一个列表，其中包含此集合的 [Task](../../com.aspose.tasks/task) 类实例。
