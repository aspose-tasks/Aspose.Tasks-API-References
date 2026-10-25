---
title: "GanttChartView.ShowBarSplits"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttChartView. يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام في مخطط جانت"
type: docs
weight: 140
url: /ar/net/aspose.tasks/ganttchartview/showbarsplits/
---
## GanttChartView.ShowBarSplits property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام في مخطط جانت.

```csharp
public bool ShowBarSplits { get; set; }
```

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

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


