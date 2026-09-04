---
title: "TaskCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة من الكائنات."
type: docs
weight: 293
url: /ar/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

يمثل مجموعة من كائنات [Task](../../com.aspose.tasks/task).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add()](#add--) | يضيف مهمة جديدة إلى مجموعة مهام المشروع على نفس المستوى الهرمي للمهمة الأخيرة. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | يدرج مهمة جديدة قبل مهمة ذات المعرف المحدد وعلى نفس المستوى الهرمي. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | أضف المهمة المحددة إلى نسخة من الفئة [TaskCollection](../../com.aspose.tasks/taskcollection). |
| [add(String taskName)](#add-java.lang.String-) | يضيف مهمة جديدة إلى مجموعة مهام الأطفال. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | يضيف مهمة متكررة جديدة إلى مجموعة مهام الأطفال. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | يتحقق مما إذا كانت المجموعة تحتوي على العنصر المحدد. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getById(int id)](#getById-int-) | إرجاع مهمة بالمعرف المحدد يكون سلفها هو المهمة الأصلية لهذه المجموعة. |
| [getByUid(int uid)](#getByUid-int-) | إرجاع مهمة بالمعرف الفريد المحدد يكون سلفها هو المهمة الأصلية لهذه المجموعة. |
| [getParentProject()](#getParentProject--) | يحصل على المشروع الأصل لكائن TaskCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |
| [iterator()](#iterator--) | يرجع مُعدِّدًا لهذه المجموعة. |
| [remove(Object item)](#remove-java.lang.Object-) | هذا هو تنفيذ تجريدي لطريقة Remove في ICollection، التي تُطلق فقط UnsupportedOperationException. |
| [size()](#size--) | يحصل على عدد الكائنات الموجودة في TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | يحول كائن TaskCollection إلى قائمة من كائنات [Task](../../com.aspose.tasks/task). |
### add() {#add--}
```
public final Task add()
```


يضيف مهمة جديدة إلى مجموعة مهام المشروع على نفس المستوى الهرمي للمهمة الأخيرة.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


يدرج مهمة جديدة قبل مهمة ذات المعرف المحدد وعلى نفس المستوى الهرمي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | المعلمات المحددة لإنشاء مهمة متكررة. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


أضف المهمة المحددة إلى نسخة من فئة [TaskCollection](../../com.aspose.tasks/taskcollection). إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحساب الحقول التابعة مثل الفجوات، والعمل، وحقول التكلفة، والمعرفات ومستويات المخطط). إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرف المهمة، ومستوى المخطط، وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، والعمل، وحقول التكلفة، ويعيد حساب المعرفات ومستويات المخطط).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | المهمة المحددة التي يجب إضافتها إلى مجموعة المهام هذه. |

**Returns:**
منطقي - true إذا كانت العملية ناجحة.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


يضيف مهمة جديدة إلى مجموعة مهام الأطفال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| taskName | java.lang.String | اسم المهمة المحدد. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


يضيف مهمة متكررة جديدة إلى مجموعة مهام الأطفال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| taskName | java.lang.String | اسم المهمة المحدد. |
| beforeTaskId | int | المعرف المحدد لمهمة يُسبقها إدراج مهمة جديدة. |

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


يتحقق مما إذا كانت المجموعة تحتوي على العنصر المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | العنصر المراد فحصه. |

**Returns:**
منطقي - صحيح إذا كانت المجموعة تحتوي على عنصر، خطأ خلاف ذلك.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\\}

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


إرجاع مهمة بالمعرف المحدد يكون سلفها هو المهمة الأصلية لهذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


إرجاع مهمة بالمعرف الفريد المحدد يكون سلفها هو المهمة الأصلية لهذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


يحصل على المشروع الأصل لكائن TaskCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


يرجع مُعدِّدًا لهذه المجموعة.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - مُعدد لهذا التجميع.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


هذا هو تنفيذ تجريدي لطريقة Remove في ICollection، التي تُطلق فقط UnsupportedOperationException.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | java.lang.Object | العنصر المراد إزالته. |

**Returns:**
منطقي - `true` إذا تم إزالة العنصر؛ `false` خلاف ذلك.
### size() {#size--}
```
public final int size()
```


يحصل على عدد الكائنات الموجودة في TaskCollection.

**Returns:**
int - عدد الكائنات الموجودة في TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


يحول كائن TaskCollection إلى قائمة من كائنات [Task](../../com.aspose.tasks/task).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - يُرجع قائمة تحتوي على مثيلات فئة [Task](../../com.aspose.tasks/task) لهذا التجميع.
