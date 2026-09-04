---
title: "OutlineValue"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل قيمة مخطط تفصيلي."
type: docs
weight: 173
url: /ar/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

يمثل قيمة مخطط تفصيلي.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDescription()](#getDescription--) | يحصل على وصف قيمة المخطط. |
| [getDurationValue()](#getDurationValue--) | يحصل على المدة إذا كان Type هو Duration. |
| [getParentValueId()](#getParentValueId--) | يحصل على Id العقدة الأم لرمز المخطط. |
| [getType()](#getType--) | يحصل على نوع رمز المخطط. |
| [getValue()](#getValue--) | يحصل على القيمة الفعلية. |
| [getValueGuid()](#getValueGuid--) | يحصل على GUID يحدد هذه القيمة بين الآخرين في المشروع بأكمله. |
| [getValueId()](#getValueId--) | يحصل على Id الفريد لقيمة رمز المخطط داخل مشروع. |
| [isCollapsed()](#isCollapsed--) | يحصل على قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | يضبط قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا. |
| [setDescription(String value)](#setDescription-java.lang.String-) | يضبط وصف قيمة المخطط. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | يضبط المدة إذا كان Type هو Duration. |
| [setParentValueId(int value)](#setParentValueId-int-) | يضبط Id العقدة الأم لرمز المخطط. |
| [setType(int value)](#setType-int-) | يضبط نوع رمز المخطط. |
| [setValue(String value)](#setValue-java.lang.String-) | يضبط القيمة الفعلية. |
| [setValueId(int value)](#setValueId-int-) | يضبط Id الفريد لقيمة رمز المخطط داخل مشروع. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


يحصل على وصف قيمة المخطط.

**Returns:**
java.lang.String - وصف قيمة المخطط.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


يحصل على المدة إذا كان Type هو Duration.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), عندما تحتاج إلى تعيين القيمة لـ OutlineValues بنوع Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


يحصل على Id العقدة الأم لرمز المخطط.

**Returns:**
int - Id العقدة الأم لرمز المخطط.
### getType() {#getType--}
```
public final int getType()
```


يحصل على نوع رمز المخطط.

**Returns:**
int - نوع رمز المخطط.
### getValue() {#getValue--}
```
public final String getValue()
```


يحصل على القيمة الفعلية.

**Returns:**
java.lang.String - القيمة الفعلية.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


يحصل على GUID يحدد هذه القيمة بين الآخرين في المشروع بأكمله.

**Returns:**
java.util.UUID - معرف GUID يحدد هذه القيمة بين القيم الأخرى في المشروع بأكمله.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


يحصل على Id الفريد لقيمة رمز المخطط داخل مشروع.

**Returns:**
int - Id الفريد لقيمة رمز المخطط داخل مشروع.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


يحصل على قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا.

--------------------

هذا جديد لخاصية MS Project 2010.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا.

--------------------

هذا جديد لخاصية MS Project 2010.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


يضبط وصف قيمة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | وصف قيمة المخطط. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


يضبط المدة إذا كان Type هو Duration.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), عندما تحتاج إلى تعيين القيمة لـ OutlineValues بنوع Duration.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | المدة إذا كان النوع هو Duration. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


يضبط Id العقدة الأم لرمز المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | معرّف العقدة الأصلية لرمز المخطط. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


يضبط نوع رمز المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع رمز المخطط. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


يضبط القيمة الفعلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة الفعلية. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


يضبط Id الفريد لقيمة رمز المخطط داخل مشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | المعرّف الفريد لقيمة رمز المخطط داخل المشروع. |

