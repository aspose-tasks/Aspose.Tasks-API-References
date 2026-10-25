---
title: "ResourceAssignmentCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة من الكائنات."
type: docs
weight: 250
url: /ar/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

يمثل مجموعة من كائنات [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | هذه هي تنفيذية النموذج لطريقة Add في ICollection، التي تُطلق فقط UnsupportedOperationException |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection. |
| [clear()](#clear--) | يزيل جميع العناصر من المجموعة. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getByUid(int uid)](#getByUid-int-) | يعيد تعيينًا بالمعرف الفريد (uid) المحدد. |
| [getParentProject()](#getParentProject--) | يحصل على المشروع الأب لكائن ResourceAssignmentCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |
| [iterator()](#iterator--) | يرجع مُعدِّدًا لهذه المجموعة. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | يزيل التعيين المحدد من المجموعة إذا لم تكن للقراءة فقط، وإلا يرمي استثناء UnsupportedOperationException. |
| [size()](#size--) | يحصل على عدد الكائنات الموجودة في ResourceAssignmentCollection. |
| [toList()](#toList--) | يحول كائن ResourceAssignmentCollection إلى قائمة من كائنات [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


هذه هي تنفيذية النموذج لطريقة Add في ICollection، التي تُطلق فقط UnsupportedOperationException

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | العنصر المراد إزالته. |

**Returns:**
منطقي - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | مهمة لتعيينها. |
| resource | [Resource](../../com.aspose.tasks/resource) | مورد لتعيينه. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | مهمة لتعيينها. |
| resource | [Resource](../../com.aspose.tasks/resource) | مورد لتعيينه. |
| الوحدات | double | عدد الوحدات لتعيين جديد. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | مهمة لتعيينها. |
| resource | [Resource](../../com.aspose.tasks/resource) | مورد تكلفة لتعيينه. |
| التكلفة | java.math.BigDecimal | التكلفة لتعيين جديد. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


يزيل جميع العناصر من المجموعة.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public ResourceAssignment get(int index)
```


(@inheritDoc\\}

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


يعيد تعيينًا بالمعرف الفريد (uid) المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | uid | int | المعرف الفريد المحدد (uid). |

--------------------

تعقيد O(1). |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


يحصل على المشروع الأب لكائن ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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
public final Iterator<ResourceAssignment> iterator()
```


يرجع مُعدِّدًا لهذه المجموعة.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - عداد لهذا التجميع.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


يزيل التعيين المحدد من المجموعة إذا لم تكن للقراءة فقط، وإلا يرمي استثناء UnsupportedOperationException.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | التعيين لإزالته. |

**Returns:**
منطقي - true إذا تم إزالة العنصر المحدد، false خلاف ذلك.
### size() {#size--}
```
public final int size()
```


يحصل على عدد الكائنات الموجودة في ResourceAssignmentCollection.

**Returns:**
int - عدد الكائنات الموجودة في ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


يحول كائن ResourceAssignmentCollection إلى قائمة من كائنات [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - قائمة من كائنات [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
