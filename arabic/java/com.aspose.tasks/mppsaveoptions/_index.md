---
title: "MPPSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند حفظ بيانات المشروع إلى MPP."
type: docs
weight: 149
url: /ar/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

يسمح بتحديد خيارات إضافية عند حفظ بيانات المشروع إلى MPP.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | ينشئ مثيلًا جديدًا للفئة [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getClearVba()](#getClearVba--) | يحصل على قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ المشروع بصيغة MPP. |
| [getProtectionPassword()](#getProtectionPassword--) | يحصل على كلمة مرور تُستخدم لحماية ملف MPP الناتج. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | يحصل على قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP. |
| [getWriteFilters()](#getWriteFilters--) | يحصل على قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلتر عند حفظ المشروع بصيغة MPP. |
| [getWriteGroups()](#getWriteGroups--) | يحصل على قيمة تشير إلى ما إذا كان يجب كتابة بيانات المجموعات عند حفظ مشروع إلى تنسيق MPP. |
| [getWriteVba()](#getWriteVba--) | يحصل على قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الموجودة في ملف MPP. |
| [getWriteViewData()](#getWriteViewData--) | يحصل على قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ مشروع إلى تنسيق MPP. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ مشروع إلى تنسيق MPP. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | يضبط كلمة مرور تُستخدم لحماية ملف MPP الناتج. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلتر عند حفظ مشروع إلى تنسيق MPP. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب كتابة بيانات المجموعات عند حفظ مشروع إلى تنسيق MPP. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الموجودة في ملف MPP. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ مشروع إلى تنسيق MPP. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


ينشئ مثيلًا جديدًا للفئة [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions).

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ المشروع بصيغة MPP.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ مشروع إلى تنسيق MPP.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


يحصل على كلمة مرور تُستخدم لحماية ملف MPP الناتج. حالياً يتم دعم ذلك لتنسيقات MS Project 2010 وما بعدها.

--------------------

القيمة الفارغة تشير إلى أن ملف المشروع غير محمي.

**Returns:**
java.lang.String - كلمة مرور تُستخدم لحماية ملف MPP الناتج.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP.

--------------------

يقوم MS Project بإنشاء تعيين مورد فارغ لكل مهمة. اضبط هذه العلامة على true لإزالتها عند الحفظ.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


يحصل على قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلتر عند حفظ المشروع بصيغة MPP.

--------------------

تشمل بيانات الفلتر مجموعات Project.TaskFilters وProject.ResourceFilters.

--------------------

مدعوم حالياً لتنسيقات MSP 2010 أو الأحدث.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلتر عند حفظ مشروع إلى تنسيق MPP.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


يحصل على قيمة تشير إلى ما إذا كان يجب كتابة بيانات المجموعات عند حفظ مشروع إلى تنسيق MPP.

--------------------

تشمل بيانات المجموعات مجموعات Project.TaskGroups وProject.ResourceGroups.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب كتابة بيانات المجموعات عند حفظ مشروع إلى تنسيق MPP.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الموجودة في ملف MPP. حالياً يتم دعم كتابة VbaModule.SourceCode.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الموجودة في ملف MPP.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


يحصل على قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ مشروع إلى تنسيق MPP.

--------------------

تشمل بيانات العرض مجموعات Project.Views وFilters وTables.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ مشروع إلى تنسيق MPP.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ مشروع إلى تنسيق MPP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الحالية عند حفظ المشروع بتنسيق MPP. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


يضبط كلمة مرور تُستخدم لحماية ملف MPP الناتج. يتم دعم ذلك حاليًا لتنسيقات MS Project 2010 والإصدارات الأحدث.

--------------------

القيمة الفارغة تشير إلى أن ملف المشروع غير محمي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | كلمة مرور تُستخدم لحماية ملف MPP الناتج. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP.

--------------------

يقوم MS Project بإنشاء تعيين مورد فارغ لكل مهمة. اضبط هذه العلامة على true لإزالتها عند الحفظ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلتر عند حفظ مشروع إلى تنسيق MPP.

--------------------

تشمل بيانات الفلتر مجموعات Project.TaskFilters وProject.ResourceFilters.

--------------------

مدعوم حالياً لتنسيقات MSP 2010 أو الأحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلاتر عند حفظ المشروع بتنسيق MPP. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب كتابة بيانات المجموعات عند حفظ مشروع إلى تنسيق MPP.

--------------------

تشمل بيانات المجموعات مجموعات Project.TaskGroups وProject.ResourceGroups.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب كتابة بيانات المجموعات عند حفظ المشروع بتنسيق MPP. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الحالية في ملف MPP. يتم دعم كتابة VbaModule.SourceCode حاليًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الحالية في ملف MPP. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ مشروع إلى تنسيق MPP.

--------------------

تشمل بيانات العرض مجموعات Project.Views وFilters وTables.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ المشروع بتنسيق MPP. |

