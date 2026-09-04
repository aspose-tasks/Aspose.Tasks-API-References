---
title: "OutlineCode"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل قيمة رمز المخطط التفصيلي."
type: docs
weight: 167
url: /ar/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

يمثل قيمة رمز المخطط التفصيلي.

--------------------

هناك عنصران من البيانات ضروريان - مؤشر إلى جدول رمز المخطط المحدد بواسطة FieldId، والقيمة المحددة إما بواسطة ValueId أو مؤشر ValueGuid إلى قائمة القيم.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | ينشئ مثلاً جديداً من الفئة [OutlineCode](../../com.aspose.tasks/outlinecode). |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | ينشئ مثلاً جديداً من الفئة [OutlineCode](../../com.aspose.tasks/outlinecode) باستخدام رمز المخطط المحدد وإحدى قيمه. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFieldId()](#getFieldId--) | يحصل على القيمة الرقمية لحقل المشروع المخصص Id. |
| [getValueGuid()](#getValueGuid--) | يحصل على GUID للقيمة في قائمة القيم. |
| [getValueId()](#getValueId--) | يحصل على Id في قائمة القيم المرتبط بالتعريف في مجموعة رمز المخطط. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | يضبط القيمة الرقمية لحقل المشروع المخصص Id. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | يضبط GUID للقيمة في قائمة القيم. |
| [setValueId(int value)](#setValueId-int-) | يضبط Id في قائمة القيم المرتبط بالتعريف في مجموعة رمز المخطط. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


ينشئ مثلاً جديداً من الفئة [OutlineCode](../../com.aspose.tasks/outlinecode).

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


ينشئ مثلاً جديداً من الفئة [OutlineCode](../../com.aspose.tasks/outlinecode) باستخدام رمز المخطط المحدد وإحدى قيمه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | تعريف رمز المخطط. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | واحدة من قيم تعريف رمز المخطط. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


يحصل على القيمة الرقمية لحقل المشروع المخصص Id.

**Returns:**
java.lang.String - القيمة العددية لحقل المشروع المخصص Id.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


يحصل على GUID القيمة في قائمة القيم. الـ ValueGuid يطابق الـ FieldGuid في قائمة القيم.

**Returns:**
java.lang.String - GUID القيمة في قائمة القيم.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


يحصل على Id في قائمة القيم المرتبط بالتعريف في مجموعة رمز المخطط.

**Returns:**
int - المعرف Id في قائمة القيم المرتبط بالتعريف في مجموعة رمز المخطط.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


يضبط القيمة الرقمية لحقل المشروع المخصص Id.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة العددية لحقل المشروع المخصص Id. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


يضبط GUID القيمة في قائمة القيم. الـ ValueGuid يطابق الـ FieldGuid في قائمة القيم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | GUID القيمة في قائمة القيم. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


يضبط Id في قائمة القيم المرتبط بالتعريف في مجموعة رمز المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | المعرف Id في قائمة القيم المرتبط بالتعريف في مجموعة رمز المخطط. |

