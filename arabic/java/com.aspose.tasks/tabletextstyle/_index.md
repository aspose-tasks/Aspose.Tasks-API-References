---
title: "TableTextStyle"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل نمط نص في جدول العرض."
type: docs
weight: 288
url: /ar/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

يمثل نمط نص في جدول العرض.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle). |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle) مع الخط المحدد. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle) مع حجم الخط المحدد ونمط الخط. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle) مع إعدادات الخط الافتراضية والنمط المحدد للخط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getField()](#getField--) | يحصل على الحقل الذي سيُطبق عليه النمط. |
| [getItemType()](#getItemType--) | يعيد نوع عنصر النص. |
| [getRowUid()](#getRowUid--) | يحصل على معرف فريد للصف. |
| [setField(int value)](#setField-int-) | يضبط الحقل الذي سيُطبق عليه النمط. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowUid | int | معرف فريد للصف المحدد. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle) مع الخط المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowUid | int | معرف فريد للصف المحدد. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | خط يُستند إليه نمط النص. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle) مع حجم الخط المحدد ونمط الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowUid | int | معرف فريد للصف المحدد. |
| fontSize | float | حجم الخط الذي يعتمد عليه نمط النص. |
| fontStyle | int | نمط الخط. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


يُهيئ مثيلاً جديداً من الفئة [TableTextStyle](../../com.aspose.tasks/tabletextstyle) مع إعدادات الخط الافتراضية والنمط المحدد للخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowUid | int | معرف فريد للصف المحدد. |
| fontStyle | int | نمط الخط. |

### getField() {#getField--}
```
public final int getField()
```


يحصل على حقل يتم تطبيق النمط عليه. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - حقل يتم تطبيق النمط عليه.
### getItemType() {#getItemType--}
```
public int getItemType()
```


يعيد نوع عنصر النص.

**Returns:**
int - قيمة النوع المعدد TextItemType.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


يحصل على معرف فريد للصف.

--------------------

أرجع -1 إذا كان النمط سيُطبق على جميع صفوف العرض.

**Returns:**
int - معرف فريد للصف.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


يضبط حقل يتم تطبيق النمط عليه. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | حقل يتم تطبيق النمط عليه. |

