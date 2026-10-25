---
title: "SaveOptions.MarkCriticalTasks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر. القيمة الافتراضية هي FALSE."
type: docs
weight: 100
url: /ar/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## الأمثلة

يوضح كيفية طباعة المهام الحرجة أثناء الحفظ بصيغ ملفات الصور.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    StartDate = project.Get(Prj.StartDate).AddDays(-3),
    EndDate = project.Get(Prj.FinishDate),
    MarkCriticalTasks = true,
    LegendDrawingOptions = LegendDrawingOptions.NoLegend,
    Gridlines = new List<Gridline>()
};

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// احفظ تخطيط المشروع إلى ملفات منفصلة
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


