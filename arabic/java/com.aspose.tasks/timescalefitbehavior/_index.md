---
title: "TimescaleFitBehavior"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل سلوكًا يُستخدم لمحاذاة منطقة مقياس الوقت مع عرض الصفحة."
type: docs
weight: 324
url: /ar/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

يمثل سلوكًا يُستخدم لمحاذاة منطقة مقياس الوقت مع عرض الصفحة.
## الحقول

| حقل | الوصف |
| --- | --- |
| [DefinedInView](#DefinedInView) | يتم عرض قسم التقويم وفقًا لخاصية View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage للعرض المُعرض. |
| [NoScaleToEndDate](#NoScaleToEndDate) | يتم عرض قسم التقويم بدقة حتى EndDate، حتى إذا كان هناك مساحة فارغة في الصفحة. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | يتم عرض قسم التقويم إلى النهاية (الجانب الأيمن) من الصفحة الأخيرة. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | سوف يحاول محرك العرض محاذاة التواريخ بحيث يكون EndDate محاذيًا مع النهاية (الجانب الأيمن) للصفحة الأخيرة. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


يتم عرض قسم التقويم وفقًا لخاصية View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage للعرض المُعرض.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


يتم عرض قسم التقويم بدقة حتى EndDate، حتى إذا كان هناك مساحة فارغة في الصفحة.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


يتم عرض قسم التقويم إلى النهاية (الجانب الأيمن) للصفحة الأخيرة. وبالتالي قد يتجاوز التاريخ المعروض الأخير EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


سوف يحاول محرك العرض محاذاة التواريخ بحيث يكون EndDate محاذيًا مع النهاية (الجانب الأيمن) للصفحة الأخيرة. يتوافق ذلك مع تمكين خيار "Page Setup \\ View \\ Fit timescale to end of page" في MS Project.

