---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 296
url: /zh/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

表示一个 [Task](../../com.aspose.tasks/task) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | 返回已添加到 TaskLinkCollection 对象的 Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) 实例。 |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | 返回已添加到 TaskLinkCollection 对象的 [TaskLink](../../com.aspose.tasks/tasklink) 实例。 |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | 返回已添加到 TaskLinkCollection 对象的 [TaskLink](../../com.aspose.tasks/tasklink) 实例。 |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 UnsupportedOperationException。 |
| [clear()](#clear--) | 保留供内部使用。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | 获取 ResourceAssignmentCollection 对象的父项目。 |
| [remove(int index)](#remove-int-) | 移除此集合中指定位置的元素，并返回被移除的元素。 |
| [remove(Object item)](#remove-java.lang.Object-) | 从项目中移除任务链接。 |
| [size()](#size--) | 返回此 `TaskLinkCollection` 对象中包含的对象数量。 |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | 将 TaskLinkCollection 对象转换为 [TaskLink](../../com.aspose.tasks/tasklink) 对象的列表。 |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


返回已添加到 TaskLinkCollection 对象的 Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 前置任务。 |
| succ | [Task](../../com.aspose.tasks/task) | 后继任务。 |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


返回已添加到 TaskLinkCollection 对象的 [TaskLink](../../com.aspose.tasks/tasklink) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 前置任务。 |
| succ | [Task](../../com.aspose.tasks/task) | 后继任务。 |
| linkType | int | 链接类型 [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


返回已添加到 TaskLinkCollection 对象的 [TaskLink](../../com.aspose.tasks/tasklink) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 前置任务。 |
| succ | [Task](../../com.aspose.tasks/task) | 后继任务。 |
| linkType | int | 链接类型 [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | 链接延迟 [Duration](../../com.aspose.tasks/duration)。 |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


这是 ICollection 的 Add 方法的存根实现，只会抛出 UnsupportedOperationException。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | 要添加的项。 |

**Returns:**
布尔 - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


保留供内部使用。

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取 ResourceAssignmentCollection 对象的父项目。

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


移除此集合中指定位置的元素，并返回被移除的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除元素的指定位置。 |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


从项目中移除任务链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | java.lang.Object | 要删除的指定 `TaskLink` 类实例。 |

**Returns:**
boolean - 返回从此集合中删除的 `TaskLink` 类实例。
### size() {#size--}
```
public final int size()
```


返回此 `TaskLinkCollection` 对象中包含的对象数量。只读 `int`。

**Returns:**
int - 返回此集合中包含的对象数量。
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


将 TaskLinkCollection 对象转换为 [TaskLink](../../com.aspose.tasks/tasklink) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - [TaskLink](../../com.aspose.tasks/tasklink) 对象的列表。
