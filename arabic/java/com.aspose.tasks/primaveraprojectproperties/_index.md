---
title: "PrimaveraProjectProperties"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثِّل الخصائص الخاصة بـ Primavera لمشروع يُقرأ من ملفات Primavera بصيغة XER أو P6XML."
type: docs
weight: 205
url: /ar/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

يمثل خصائص خاصة بـ Primavera لمشروع يُقرأ من ملفات Primavera (XER أو P6XML).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | يحصل على مصفوفة من مشاريع الأساس للمشروع الحالي. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | يحصل على الطريقة المستخدمة لتحديد الأنشطة الحرجة: المسار الأطول أو نهج الفاصل الكلي. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | يحصل على قيمة العتبة المستخدمة لتحديد الأنشطة الحرجة إذا تم استخدام طريقة TotalFloat. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | يحصل على معرّف مشروع الأساس الحالي. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | يحصل على علم يحدد ما إذا كان يجب تجاهل علاقات الأنشطة بين المشاريع. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | يحصل على علم يحدد ما إذا كان يجب وضع علامة على الأنشطة كحرجة عند جدولة المشروع. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | يحصل على خيار يحدد أي تقويم يُستخدم لجدولة تأخر العلاقة في مشاريع Primavera. |
| [getShortName()](#getShortName--) | يحصل على الاسم المختصر للمشروع (معرّف المشروع). |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | يحصل على علم يحدد ما إذا كان يجب جدولة تواريخ انتهاء الأنشطة كتواريخ الانتهاء المتوقعة. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


يحصل على مصفوفة من مشاريع الأساس للمشروع الحالي. ينطبق على المشاريع التي تُقرأ من ملفات Primavera XML التي تحتوي على أسس مُصدَّرة.

**Returns:**
com.aspose.tasks.Project[] - مصفوفة من مشاريع الأساس للمشروع الحالي.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


يحصل على الطريقة المستخدمة لتحديد الأنشطة الحرجة: المسار الأطول أو نهج الفاصل الكلي.

**Returns:**
int - الطريقة المستخدمة لتحديد الأنشطة الحرجة: المسار الأطول أو نهج الفاصل الكلي.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


يحصل على قيمة العتبة المستخدمة لتحديد الأنشطة الحرجة إذا تم استخدام طريقة TotalFloat.

**Returns:**
java.lang.Double - قيمة العتبة المستخدمة لتحديد الأنشطة الحرجة إذا تم استخدام طريقة TotalFloat.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


يحصل على معرّف مشروع الأساس الحالي. ينطبق على المشاريع التي تُقرأ من ملفات Primavera XML التي تحتوي على أسس مُصدَّرة.

**Returns:**
int - معرف المشروع الأساسي الحالي.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


يحصل على علم يحدد ما إذا كان يجب تجاهل علاقات الأنشطة بين المشاريع.

**Returns:**
boolean - علم يحدد ما إذا كان يجب تجاهل علاقات الأنشطة بين المشاريع.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


يحصل على علم يحدد ما إذا كان يجب وضع علامة على الأنشطة كحرجة عند جدولة المشروع.

**Returns:**
boolean - علم يحدد ما إذا كان يجب وضع علامة على الأنشطة كحرجة عند جدولة المشروع.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


يحصل على خيار يحدد أي تقويم يُستخدم لجدولة تأخر العلاقة في مشاريع Primavera.

**Returns:**
int - خيار يحدد أي تقويم يُستخدم لجدولة تأخر العلاقة في مشاريع Primavera.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


يحصل على الاسم المختصر للمشروع (معرّف المشروع).

**Returns:**
java.lang.String - الاسم المختصر للمشروع (معرّف المشروع).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


يحصل على علم يحدد ما إذا كان يجب جدولة تواريخ انتهاء الأنشطة كتواريخ الانتهاء المتوقعة.

**Returns:**
boolean - علم يحدد ما إذا كان يجب جدولة تواريخ انتهاء الأنشطة كتواريخ الانتهاء المتوقعة.
