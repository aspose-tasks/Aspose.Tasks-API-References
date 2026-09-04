---
title: "ViewColumn"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل عمودًا في عرض المشروع."
type: docs
weight: 344
url: /ar/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

يمثل عمودًا في عرض المشروع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getField()](#getField--) | يحصل على حقل العمود. |
| [getName()](#getName--) | يحصل على اسم العمود. |
| [getStringAlignment()](#getStringAlignment--) | يحصل على محاذاة النص (يمكن أن تكون واحدة من قيم تعداد [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | يحصل على رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود. |
| [getWidth()](#getWidth--) | يحصل على عرض العمود. |
| [setField(int value)](#setField-int-) | يضبط حقل العمود. |
| [setStringAlignment(int value)](#setStringAlignment-int-) | يضبط محاذاة النص (يمكن أن تكون واحدة من قيم تعداد [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment)). |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | يضبط رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود. |
### getField() {#getField--}
```
public abstract int getField()
```


يحصل على حقل العمود. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - حقل العمود.
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم العمود.

**Returns:**
java.lang.String - اسم العمود.
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


يحصل على محاذاة النص (يمكن أن تكون واحدة من قيم تعداد [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - محاذاة النص (يمكن أن تكون واحدة من قيم تعداد [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


يحصل على رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود.

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


يحصل على عرض العمود.

**Returns:**
int - عرض العمود.
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


يضبط حقل العمود. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | حقل العمود. |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


يضبط محاذاة النص (يمكن أن تكون واحدة من قيم تعداد [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | محاذاة النص (يمكن أن تكون واحدة من قيم تعداد [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


يضبط رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود. |

