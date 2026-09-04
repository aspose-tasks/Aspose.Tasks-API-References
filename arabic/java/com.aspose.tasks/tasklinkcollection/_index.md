---
title: "TaskLinkCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة من الكائنات."
type: docs
weight: 296
url: /ar/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

يمثل مجموعة من كائنات [Task](../../com.aspose.tasks/task).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | يعيد مثيلاً من نوع Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) تم إضافته إلى كائن TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | يعيد مثيلاً من [TaskLink](../../com.aspose.tasks/tasklink) تم إضافته إلى كائن TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | يعيد مثيلاً من [TaskLink](../../com.aspose.tasks/tasklink) تم إضافته إلى كائن TaskLinkCollection. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | هذه هي تنفيذية النموذج لطريقة Add في ICollection، التي تُطلق فقط UnsupportedOperationException |
| [clear()](#clear--) | محجوز للاستخدام الداخلي. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getParentProject()](#getParentProject--) | يحصل على المشروع الأب لكائن ResourceAssignmentCollection. |
| [remove(int index)](#remove-int-) | يزيل العنصر في الموضع المحدد في هذه المجموعة ويعيد العنصر الذي تم إزالته من المجموعة. |
| [remove(Object item)](#remove-java.lang.Object-) | يزيل رابط المهمة من مشروع. |
| [size()](#size--) | يعيد عدد الكائنات الموجودة في هذا الكائن `TaskLinkCollection`. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | يحوّل كائن TaskLinkCollection إلى قائمة من كائنات [TaskLink](../../com.aspose.tasks/tasklink). |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


يعيد مثيلاً من نوع Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) تم إضافته إلى كائن TaskLinkCollection.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | مهمة سابقة. |
| succ | [Task](../../com.aspose.tasks/task) | مهمة لاحقة. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


يعيد مثيلاً من [TaskLink](../../com.aspose.tasks/tasklink) تم إضافته إلى كائن TaskLinkCollection.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | مهمة سابقة. |
| succ | [Task](../../com.aspose.tasks/task) | مهمة لاحقة. |
| linkType | int | نوع الارتباط [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


يعيد مثيلاً من [TaskLink](../../com.aspose.tasks/tasklink) تم إضافته إلى كائن TaskLinkCollection.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | مهمة سابقة. |
| succ | [Task](../../com.aspose.tasks/task) | مهمة لاحقة. |
| linkType | int | نوع الارتباط [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | تأخير الارتباط [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


هذه هي تنفيذية النموذج لطريقة Add في ICollection، التي تُطلق فقط UnsupportedOperationException

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | العنصر المراد إضافته. |

**Returns:**
منطقي - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


محجوز للاستخدام الداخلي.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\\}

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


يحصل على المشروع الأب لكائن ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


يزيل العنصر في الموضع المحدد في هذه المجموعة ويعيد العنصر الذي تم إزالته من المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الموضع المحدد لإزالة العنصر عنده. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


يزيل رابط المهمة من مشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | java.lang.Object | مثيل `TaskLink` المحدد للإزالة. |

**Returns:**
منطقي - يعيد مثيل فئة `TaskLink` الذي تمت إزالته من هذه المجموعة.
### size() {#size--}
```
public final int size()
```


يعيد عدد الكائنات الموجودة في هذا الكائن `TaskLinkCollection`. قراءة فقط `int`.

**Returns:**
`int` - يعيد عدد الكائنات الموجودة في هذه المجموعة.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


يحوّل كائن TaskLinkCollection إلى قائمة من كائنات [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
`java.util.List&lt;com.aspose.tasks.TaskLink&gt;` - قائمة من كائنات [TaskLink](../../com.aspose.tasks/tasklink).
