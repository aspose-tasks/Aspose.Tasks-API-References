---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 컬렉션을 나타냅니다."
type: docs
weight: 296
url: /ko/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

[Task](../../com.aspose.tasks/task) 객체의 컬렉션을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) 인스턴스를 반환하며, 해당 인스턴스는 TaskLinkCollection 객체에 추가됩니다. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | [TaskLink](../../com.aspose.tasks/tasklink) 인스턴스를 반환하며, 해당 인스턴스는 TaskLinkCollection 객체에 추가됩니다. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | [TaskLink](../../com.aspose.tasks/tasklink) 인스턴스를 반환하며, 해당 인스턴스는 TaskLinkCollection 객체에 추가됩니다. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | ICollection의 Add 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다. |
| [clear()](#clear--) | 내부 사용을 위해 예약됨. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection 객체의 상위 프로젝트를 가져옵니다. |
| [remove(int index)](#remove-int-) | 이 컬렉션에서 지정된 위치에 있는 요소를 제거하고, 제거된 요소를 반환합니다. |
| [remove(Object item)](#remove-java.lang.Object-) | 프로젝트에서 작업 링크를 제거합니다. |
| [size()](#size--) | `TaskLinkCollection` 객체에 포함된 객체 수를 반환합니다. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskLinkCollection 객체를 [TaskLink](../../com.aspose.tasks/tasklink) 객체 목록으로 변환합니다. |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) 인스턴스를 반환하며, 해당 인스턴스는 TaskLinkCollection 객체에 추가됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 선행 작업. |
| succ | [Task](../../com.aspose.tasks/task) | 후속 작업. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


[TaskLink](../../com.aspose.tasks/tasklink) 인스턴스를 반환하며, 해당 인스턴스는 TaskLinkCollection 객체에 추가됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 선행 작업. |
| succ | [Task](../../com.aspose.tasks/task) | 후속 작업. |
| linkType | int | 링크 유형 [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


[TaskLink](../../com.aspose.tasks/tasklink) 인스턴스를 반환하며, 해당 인스턴스는 TaskLinkCollection 객체에 추가됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 선행 작업. |
| succ | [Task](../../com.aspose.tasks/task) | 후속 작업. |
| linkType | int | 링크 유형 [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | 링크 지연 [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


ICollection의 Add 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | 추가할 항목. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


내부 사용을 위해 예약됨.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection 객체의 상위 프로젝트를 가져옵니다.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


이 컬렉션에서 지정된 위치에 있는 요소를 제거하고, 제거된 요소를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 요소를 제거할 지정된 위치. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


프로젝트에서 작업 링크를 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | java.lang.Object | 제거할 `TaskLink` 클래스의 지정된 인스턴스. |

**Returns:**
boolean - 이 컬렉션에서 제거된 `TaskLink` 클래스의 인스턴스를 반환합니다.
### size() {#size--}
```
public final int size()
```


`TaskLinkCollection` 객체에 포함된 객체 수를 반환합니다. 읽기 전용 `int`.

**Returns:**
int - 이 컬렉션에 포함된 객체 수를 반환합니다.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


TaskLinkCollection 객체를 [TaskLink](../../com.aspose.tasks/tasklink) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - [TaskLink](../../com.aspose.tasks/tasklink) 객체 목록.
