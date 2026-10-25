---
title: "CustomProjectPropertyCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة من الخصائص المخصصة للمشروع."
type: docs
weight: 61
url: /ar/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

يمثل مجموعة من الخصائص المخصصة للمشروع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | ينشئ مثلاً جديداً من الفئة [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | ينشئ خاصية مخصصة جديدة. |
| [add(String name, double value)](#add-java.lang.String-double-) | ينشئ خاصية مخصصة جديدة. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | ينشئ خاصية مخصصة جديدة. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | ينشئ خاصية مخصصة جديدة. |
| [clear()](#clear--) | يمسح PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [remove(String name)](#remove-java.lang.String-) | يزيل خاصية بالاسم المحدد من المجموعة. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


ينشئ مثلاً جديداً من الفئة [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection).

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


ينشئ خاصية مخصصة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | منطقي | قيمة كائن الخاصية الذي تم إنشاؤه حديثاً. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


ينشئ خاصية مخصصة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | double | قيمة كائن الخاصية الذي تم إنشاؤه حديثاً. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


ينشئ خاصية مخصصة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | java.lang.String | قيمة كائن الخاصية الذي تم إنشاؤه حديثاً. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


ينشئ خاصية مخصصة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية. |
| القيمة | java.util.Date | قيمة كائن الخاصية الذي تم إنشاؤه حديثاً. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


يمسح PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


يزيل خاصية بالاسم المحدد من المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف. |

**Returns:**
منطقي - True إذا تم العثور على العنصر وإزالته بنجاح؛ وإلا، false.
