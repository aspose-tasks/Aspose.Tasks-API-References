---
title: "ViewCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحتوي على قائمة من الكائنات."
type: docs
weight: 343
url: /ar/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

يحتوي على قائمة من كائنات [View](../../com.aspose.tasks/view). يمتد من الفئة `AbstractCollection`.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [clear()](#clear--) | يزيل جميع العناصر من هذه المجموعة. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [getByName(String viewName)](#getByName-java.lang.String-) | يبحث عن View بالاسم، ويعيد أول ظهور داخل المجموعة. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | يبحث عن View بالخاصية Screen المحددة، ويعيد أول ظهور داخل المجموعة. |
| [getParentProject()](#getParentProject--) | يحصل على الأصل لكائن View. |
| [iterator()](#iterator--) | يعيد مكرّرًا على العناصر الموجودة في هذه المجموعة. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | يزيل أول ظهور لكائن محدد من هذه المجموعة. |
| [size()](#size--) | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [toList()](#toList--) | يحوّل مجموعة العرض إلى قائمة من كائنات [View](../../com.aspose.tasks/view). |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


يضيف العنصر المحدد إلى هذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | العنصر المحدد لإضافته إلى هذه المجموعة. |

**Returns:**
boolean - true إذا كانت العملية ناجحة.
### clear() {#clear--}
```
public final void clear()
```


يزيل جميع العناصر من هذه المجموعة.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | العنصر المحدد للبحث عنه. |

**Returns:**
منطقي - true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | المصفوفة الأحادية الأبعاد المحددة لنسخ العناصر إليها |
| arrayIndex | int | الفهرس الصفري للمصفوفة المحددة الذي يبدأ عنده النسخ. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


يبحث عن View بالاسم، ويعيد أول ظهور داخل المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| viewName | java.lang.String | اسم الـ View للبحث. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


يبحث عن View بالخاصية Screen المحددة، ويعيد أول ظهور داخل المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| screen | int | قيمة تعداد [ViewScreen](../../com.aspose.tasks/viewscreen). |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


يحصل على الأصل لكائن View. للقراءة فقط [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


يعيد مكرّرًا على العناصر الموجودة في هذه المجموعة.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - مكرّر المجموعة.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


يزيل أول ظهور لكائن محدد من هذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | الكائن المحدد للإزالة. |

**Returns:**
boolean - true إذا تم إزالة الكائن المحدد بنجاح من هذا التجميع؛ وإلا false.
### size() {#size--}
```
public final int size()
```


يحصل على عدد العناصر الموجودة في هذه المجموعة.

**Returns:**
int - عدد العناصر الموجودة في هذه المجموعة.
### toList() {#toList--}
```
public final List<View> toList()
```


يحوّل مجموعة العرض إلى قائمة من كائنات [View](../../com.aspose.tasks/view).

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - قائمة عامة من كائنات [View](../../com.aspose.tasks/view).
