---
title: "FieldHelper"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة المساعدة التي توفر عمليات مفيدة مع الحقول."
type: docs
weight: 88
url: /ar/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

فئة المساعدة التي توفر عمليات مفيدة مع الحقول.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | يرجع عنوانًا افتراضيًا للحقل المحدد. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | يعيد عنوانًا افتراضيًا لحقل المهمة المحدد. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


يرجع عنوانًا افتراضيًا للحقل المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| حقل | int | حقل للحصول على عنوان افتراضي. |

**Returns:**
java.lang.String - عنوان افتراضي للحقل المحدد إذا كان يمكن عرض الحقل في عرض MS Project، وإلا يكون null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


يعيد عنوانًا افتراضيًا لحقل المهمة المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| taskKey | byte | حقل المهمة للحصول على عنوان افتراضي. |

**Returns:**
java.lang.String - عنوان افتراضي لحقل المهمة المحدد إذا كان يمكن عرض الحقل في عرض MS Project، وإلا يكون null.
