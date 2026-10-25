---
title: "PrimaveraSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند حفظ المشروع بتنسيق Primavera XER."
type: docs
weight: 208
url: /ar/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

يسمح بتحديد خيارات إضافية عند حفظ المشروع بتنسيق Primavera XER.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | ينشئ مثيلًا جديدًا من الفئة [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | يحصل على الزيادة المستخدمة في إعادة ترقيم معرفات النشاط. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | يحصل على البادئة المستخدمة في إعادة ترقيم معرفات النشاط. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | يحصل على اللاحقة المستخدمة في إعادة ترقيم معرفات النشاط. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | يحصل على قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرفات النشاط. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | يحصل على قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | يضبط الزيادة المستخدمة في إعادة ترقيم معرفات النشاط. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | يضبط البادئة المستخدمة في إعادة ترقيم معرفات النشاط. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | يضبط اللاحقة المستخدمة في إعادة ترقيم معرفات النشاط. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | يضبط قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرّفات النشاط. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


ينشئ مثيلًا جديدًا من الفئة [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


يحصل على الزيادة المستخدمة في إعادة ترقيم معرفات النشاط.

**Returns:**
int - الزيادة المستخدمة في إعادة ترقيم معرّفات النشاط.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


يحصل على البادئة المستخدمة في إعادة ترقيم معرفات النشاط.

**Returns:**
java.lang.String - البادئة المستخدمة في إعادة ترقيم معرّفات النشاط.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


يحصل على اللاحقة المستخدمة في إعادة ترقيم معرفات النشاط.

**Returns:**
int - اللاحقة المستخدمة في إعادة ترقيم معرّفات النشاط.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


يحصل على قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرفات النشاط.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرّفات النشاط.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير.

برنامج Primavera لا يدعم تعيين الموارد إلى مهام الملخص (WBS). وبالتالي، قد يؤدي تصدير هذه التعيينات إلى ملف غير صالح وفقًا لنموذج Primavera. إذا كان true، يتم تخطي التعيينات إلى مهام الملخص أثناء التصدير. إذا كان false (القيمة الافتراضية)، سيتم رمي استثناء إذا تم مواجهة تعيين إلى مهمة ملخص أثناء التصدير.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


يضبط الزيادة المستخدمة في إعادة ترقيم معرفات النشاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الزيادة المستخدمة في إعادة ترقيم معرّفات النشاط. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


يضبط البادئة المستخدمة في إعادة ترقيم معرفات النشاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | البادئة المستخدمة في إعادة ترقيم معرّفات النشاط. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


يضبط اللاحقة المستخدمة في إعادة ترقيم معرفات النشاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | اللاحقة المستخدمة في إعادة ترقيم معرّفات النشاط. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرّفات النشاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرّفات النشاط. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير.

برنامج Primavera لا يدعم تعيين الموارد إلى مهام الملخص (WBS). وبالتالي، قد يؤدي تصدير هذه التعيينات إلى ملف غير صالح وفقًا لنموذج Primavera. إذا كان true، يتم تخطي التعيينات إلى مهام الملخص أثناء التصدير. إذا كان false (القيمة الافتراضية)، سيتم رمي استثناء إذا تم مواجهة تعيين إلى مهمة ملخص أثناء التصدير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير. |

