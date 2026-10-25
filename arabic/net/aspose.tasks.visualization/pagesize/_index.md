---
title: "تعداد PageSize"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.Visualization.PageSize enum. يحدد حجم الصفحة"
type: docs
weight: 3250
url: /ar/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

يحدد حجم الصفحة.

```csharp
public enum PageSize
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Letter | `0` | حجم صفحة Letter بالنقاط هو 792 × 612 |
| Ledger | `1` | حجم صفحة Ledger بالنقاط هو 1224 × 792 |
| A0 | `2` | حجم صفحة A0 بالنقاط هو 3371 × 2384 |
| A1 | `3` | حجم صفحة A1 بالنقاط هو 2384 × 1685 |
| A2 | `4` | حجم صفحة A2 بالنقاط هو 1684 × 1190 |
| A3 | `5` | حجم صفحة A3 بالنقاط هو 1190 × 842 |
| A4 | `6` | حجم صفحة A4 بالنقاط هو 842 × 595 |
| DefinedInView | `7` | استخدم حجم الصفحة المحدد في View's [`PageSettings`](../pagesettings/) (View.PageInfo.PageSettings). |

## الأمثلة

يظهر كيفية تعيين قيمة تشير إلى أن المهام الفرعية على شريط مهمة الملخص يجب تجميعها.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // أو
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


