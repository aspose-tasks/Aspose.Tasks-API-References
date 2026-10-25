---
title: "SaveOptions.Gridlines"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يضبط قائمة من Gridline التي تظهر في عرض المشروع"
type: docs
weight: 60
url: /ar/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

يحصل أو يضبط قائمة من [`Gridline`](../../../aspose.tasks.visualization/gridline/) التي تظهر في عرض المشروع.

```csharp
public List<Gridline> Gridlines { get; set; }
```

## الأمثلة

يوضح كيفية حفظ التخطيط إلى ملفات منفصلة.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// احفظ تخطيط المشروع إلى ملفات منفصلة
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### انظر أيضًا

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


