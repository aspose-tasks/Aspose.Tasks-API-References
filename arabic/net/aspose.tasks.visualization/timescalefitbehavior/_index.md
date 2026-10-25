---
title: "التعداد TimescaleFitBehavior"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Visualization.TimescaleFitBehavior. يمثل سلوكًا يُستخدم لمحاذاة منطقة مقياس الوقت مع عرض الصفحة."
type: docs
weight: 3440
url: /ar/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

يمثل سلوكًا يُستخدم لمحاذاة منطقة مقياس الوقت مع عرض الصفحة.

```csharp
public enum TimescaleFitBehavior
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DefinedInView | `0` | يتم عرض قسم التقويم وفقًا لخاصية View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage في العرض المُعرض. |
| NoScaleToEndDate | `1` | يتم عرض قسم التقويم بدقة حتى تاريخ الانتهاء، حتى وإن كان هناك مساحة فارغة في الصفحة. |
| NoScaleToEndOfPage | `2` | يتم عرض قسم التقويم إلى النهاية (الجانب الأيمن) للصفحة الأخيرة. وبالتالي قد يتجاوز التاريخ المعروض الأخير تاريخ الانتهاء. |
| ScaleToEndOfPage | `3` | سوف يحاول محرك العرض محاذاة التواريخ بحيث يكون تاريخ الانتهاء محاذيًا مع النهاية (الجانب الأيمن) للصفحة الأخيرة. يتطابق مع تمكين خيار "إعداد الصفحة \\ عرض \\ ملاءمة مقياس الوقت إلى نهاية الصفحة" في MS Project. |

## الأمثلة

يوضح كيفية استخدام TimescaleFitBehavior لجعل مقياس وقت مخطط جانت يتلاءم مع نهاية الصفحة الأخيرة.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


