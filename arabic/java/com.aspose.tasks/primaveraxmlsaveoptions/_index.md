---
title: "PrimaveraXmlSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند حفظ المشروع بتنسيق Primavera xml."
type: docs
weight: 212
url: /ar/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

يسمح بتحديد خيارات إضافية عند حفظ المشروع بتنسيق Primavera xml.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | ينشئ مثيلاً جديداً من الفئة [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | يحصل على قيمة تشير إلى ما إذا كان يجب حفظ مهمة جذر أم لا. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | يحصل على قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب حفظ مهمة جذر أم لا. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


ينشئ مثيلاً جديداً من الفئة [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


يحصل على قيمة تشير إلى ما إذا كان يجب حفظ مهمة جذر أم لا.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب حفظ مهمة جذر أم لا.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير.

برنامج Primavera لا يدعم تعيين الموارد إلى مهام الملخص (WBS). وبالتالي، قد يؤدي تصدير هذه التعيينات إلى ملف غير صالح وفقًا لنموذج Primavera. إذا كان true، يتم تخطي التعيينات إلى مهام الملخص أثناء التصدير. إذا كان false (القيمة الافتراضية)، سيتم رمي استثناء إذا تم مواجهة تعيين إلى مهمة ملخص أثناء التصدير.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى مهام الملخص أثناء التصدير.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب حفظ مهمة جذر أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب حفظ مهمة جذر أم لا. |

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

