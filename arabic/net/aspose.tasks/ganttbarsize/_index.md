---
title: "التعداد GanttBarSize"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.GanttBarSize. يحدد ارتفاع الشريط بالنقاط"
type: docs
weight: 700
url: /ar/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

يحدد ارتفاع الشريط بالنقاط.

```csharp
public enum GanttBarSize
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| BarSize6 | `0` | حجم الشريط 6 نقاط. |
| BarSize8 | `1` | حجم الشريط 8 نقاط. |
| BarSize10 | `2` | حجم الشريط 10 نقاط. |
| BarSize12 | `3` | حجم الشريط 12 نقاط. |
| BarSize14 | `4` | حجم الشريط 14 نقاط. |
| BarSize18 | `5` | حجم الشريط 18 نقاط. |
| BarSize24 | `6` | حجم الشريط 24 نقاط. |

## الأمثلة

يعرض كيفية تعيين بعض الخصائص المفيدة لعرض مخطط جانت.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// تعيين قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم
view.BarRounding = false;
// تعيين الارتفاع، بالنقاط، لأشرطة جانت في مخطط جانت
view.BarSize = GanttBarSize.BarSize24;
// تعيين قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص
view.HideRollupBarsWhenSummaryExpanded = true;
// تعيين لون وقت غير العمل
view.NonWorkingTimeColor = Color.Azure;
// تعيين قيمة تشير إلى ما إذا كان يجب تجميع الأشرطة على مخطط جانت
view.RollUpGanttBars = true;
// تعيين قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهمة على مخطط جانت
view.ShowBarSplits = true;
// تعيين قيمة تشير إلى ما إذا كان يجب إظهار الرسومات على مخطط جانت
view.ShowDrawings = true;
// تعيين نسبة لتقليل أو تكبير المسافة بين الوحدات على مستوى مقياس الزمن
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


