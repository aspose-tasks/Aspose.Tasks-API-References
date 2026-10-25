---
title: "PrimaveraProjectInfo"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل معلومات مختصرة عن مشروع تم تحميله من تنسيق Primavera."
type: docs
weight: 204
url: /ar/java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

يمثل معلومات مختصرة عن مشروع تم تحميله من تنسيق Primavera.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | يحصل على علامة تصدير المشروع. |
| [getName()](#getName--) | يحصل على اسم المشروع. |
| [getShortName()](#getShortName--) | يحصل على الاسم المختصر للمشروع (معرّف المشروع). |
| [getUid()](#getUid--) | يحصل على معرّف المشروع. |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


يحصل على علامة تصدير المشروع. عندما يتم اختيار مشروع للتصدير في Primavera، تكون قيمة ExportFlag الخاصة به true. قد يتم تصدير بعض المشاريع التي لم يتم اختيارها صراحةً إلى ملف XER بسبب ارتباطها بالمشروع المُصدَّر.

**Returns:**
منطقي - علامة تصدير المشروع.
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم المشروع.

**Returns:**
java.lang.String - اسم المشروع.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


يحصل على الاسم المختصر للمشروع (معرّف المشروع).

**Returns:**
java.lang.String - الاسم المختصر للمشروع (معرّف المشروع).
### getUid() {#getUid--}
```
public final int getUid()
```


يحصل على معرّف المشروع.

**Returns:**
int - معرّف المشروع.
