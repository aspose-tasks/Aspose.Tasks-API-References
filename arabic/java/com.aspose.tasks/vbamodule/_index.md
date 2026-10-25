---
title: "VbaModule"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل وحدة VBA."
type: docs
weight: 334
url: /ar/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

يمثل وحدة VBA.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | ينشئ نسخة من [VbaModule](../../com.aspose/tasks/vbamodule) من النوع VbaModuleType.ClassModule. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | ينشئ نسخة من [VbaModule](../../com.aspose/tasks/vbamodule) من النوع VbaModuleType.ProceduralModule. |
| [getAttributes()](#getAttributes--) | يسترجع مجموعة من سمات الوحدة. |
| [getName()](#getName--) | يسترجع اسم وحدة VBA |
| [getSourceCode()](#getSourceCode--) | يسترجع شفرة المصدر لوحدة VBA |
| [getType()](#getType--) | يسترجع نوع الوحدة. |
| [setName(String value)](#setName-java.lang.String-) | اسم وحدة VBA |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | يضبط شفرة المصدر لوحدة VBA |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


ينشئ نسخة من [VbaModule](../../com.aspose/tasks/vbamodule) من النوع VbaModuleType.ClassModule.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


ينشئ نسخة من [VbaModule](../../com.aspose/tasks/vbamodule) من النوع VbaModuleType.ProceduralModule.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


يسترجع مجموعة من سمات الوحدة.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


يسترجع اسم وحدة VBA

**Returns:**
java.lang.String - اسم وحدة VBA
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


يسترجع شفرة المصدر لوحدة VBA

**Returns:**
java.lang.String - شفرة المصدر لوحدة VBA
### getType() {#getType--}
```
public final int getType()
```


يسترجع نوع الوحدة.

**Returns:**
int - نوع الوحدة.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


اسم وحدة VBA

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم وحدة VBA |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


يضبط شفرة المصدر لوحدة VBA

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | شفرة المصدر لوحدة VBA |

