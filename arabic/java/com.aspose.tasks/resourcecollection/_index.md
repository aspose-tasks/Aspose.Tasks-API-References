---
title: "ResourceCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة من الكائنات."
type: docs
weight: 251
url: /ar/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

يمثل مجموعة من كائنات [Resource](../../com.aspose/tasks/resource).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add()](#add--) | يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | يضيف موردًا جديدًا في الموضع المحدد لمجموعة موارد المشروع. |
| [clear()](#clear--) | المسح المباشر غير مدعوم، هذه الطريقة فقط تُطلق استثناء UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getById(int id)](#getById-int-) | يعيد موردًا بالمعرف المحدد. |
| [getByUid(int uid)](#getByUid-int-) | يعيد موردًا بالمعرف الفريد المحدد. |
| [getParentProject()](#getParentProject--) | يحصل على المشروع الأب لكائن ResourceCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | يرجع مُعدِّدًا لهذه المجموعة. |
| [remove(Object o)](#remove-java.lang.Object-) | هذه هي تنفيذية النموذج الأولي لطريقة remove في Collection، التي فقط تُطلق UnsupportedOperationException. |
| [size()](#size--) | يحصل على عدد العناصر الموجودة في ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | يحول كائن ResourceCollection إلى قائمة من كائنات [Resource](../../com.aspose.tasks/resource). |
### add() {#add--}
```
public final Resource add()
```


يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| resourceName | java.lang.String | اسم المورد. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


يضيف موردًا جديدًا في الموضع المحدد لمجموعة موارد المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| resourceName | java.lang.String | اسم المورد. |
| beforeResourceId | int | موضع المورد السابق في مجموعة موارد المشروع. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


المسح المباشر غير مدعوم، هذه الطريقة فقط تُطلق استثناء UnsupportedOperationException.

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
public Resource get(int index)
```


(@inheritDoc\\}

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


يعيد موردًا بالمعرف المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | id | int | المعرف المحدد. |

--------------------

تعقيد O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


يعيد موردًا بالمعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | uid | int | المعرف الفريد المحدد (uid). |

--------------------

تعقيد O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


يحصل على المشروع الأب لكائن ResourceCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
منطقي - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


يرجع مُعدِّدًا لهذه المجموعة.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - عداد لهذه المجموعة.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


هذه هي تنفيذية النموذج الأولي لطريقة remove في Collection، التي فقط تُطلق UnsupportedOperationException.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | العنصر المراد إزالته. |

**Returns:**
منطقي - `true` إذا تم إزالة العنصر؛ `false` خلاف ذلك.
### size() {#size--}
```
public final int size()
```


يحصل على عدد العناصر الموجودة في ResourceCollection.

--------------------

`int` للقراءة فقط.

**Returns:**
int - عدد العناصر الموجودة في ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


يحول كائن ResourceCollection إلى قائمة من كائنات [Resource](../../com.aspose.tasks/resource).

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - قائمة من كائنات [Resource](../../com.aspose.tasks/resource).
