---
title: "PrimaveraReadOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند قراءة ملفات Primavera Xml أو Primavera Xer."
type: docs
weight: 206
url: /ar/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

يسمح بتحديد خيارات إضافية عند قراءة ملفات Primavera Xml أو Primavera Xer.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | يُنشئ مثلاً جديداً من الفئة [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | يحصل على علم يحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات. |
| [getProjectUid()](#getProjectUid--) | يحصل على معرف UID لمشروع لقراءته من ملف يحتوي على مشاريع متعددة. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | يحصل على علم يحدد ما إذا كان يجب تحميل مشاريع الخط الأساسي. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | يحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | يضبط علامة تحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات. |
| [setProjectUid(int value)](#setProjectUid-int-) | يضبط معرف UID لمشروع لقراءته من ملف يحتوي على مشاريع متعددة. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | يضبط علامة تحدد ما إذا كان يجب تحميل مشاريع الخط الأساسي. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | يحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


يُنشئ مثلاً جديداً من الفئة [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions).

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


يحصل على علم يحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات.

**Returns:**
boolean - علامة تحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


يحصل على معرف UID لمشروع لقراءته من ملف يحتوي على مشاريع متعددة.

**Returns:**
int - معرف UID لمشروع لقراءته من ملف يحتوي على مشاريع متعددة.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


يحصل على علامة تحدد ما إذا كان يجب تحميل مشاريع الخط الأساسي. القيمة الافتراضية هي true.

--------------------

العلم ينطبق على ملفات Primavera XML التي تحتوي على مشاريع الخط الأساسي (الخطوط الأساسية غير مدعومة في تنسيق XER). يمكن ضبط الخيار على false لتسريع تحميل مشروع كبير يحتوي على خطوط أساسية عندما لا تكون بيانات الخط الأساسي مطلوبة.

**Returns:**
boolean - علامة تحدد ما إذا كان يجب تحميل مشاريع الخط الأساسي.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


يحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER.

**Returns:**
int - السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


يضبط علامة تحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | علامة تحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


يضبط معرف UID لمشروع لقراءته من ملف يحتوي على مشاريع متعددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | معرف UID لمشروع لقراءته من ملف يحتوي على مشاريع متعددة. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


يضبط علامة تحدد ما إذا كان يجب تحميل مشاريع الخط الأساسي. القيمة الافتراضية هي true.

--------------------

العلم ينطبق على ملفات Primavera XML التي تحتوي على مشاريع الخط الأساسي (الخطوط الأساسية غير مدعومة في تنسيق XER). يمكن ضبط الخيار على false لتسريع تحميل مشروع كبير يحتوي على خطوط أساسية عندما لا تكون بيانات الخط الأساسي مطلوبة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | علامة تحدد ما إذا كان يجب تحميل مشاريع الخط الأساسي. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


يحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER. |

