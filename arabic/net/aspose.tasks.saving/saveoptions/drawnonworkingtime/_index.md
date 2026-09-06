---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد قيمة تشير إلى ما إذا كان يجب رسم وقت غير العمل. القيمة الافتراضية هي TRUE."
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب رسم وقت عدم العمل (القيمة الافتراضية هي TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


