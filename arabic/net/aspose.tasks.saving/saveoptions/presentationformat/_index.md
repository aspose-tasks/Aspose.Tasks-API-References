---
title: "SaveOptions.PresentationFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يضبط الـ PresentationFormat الذي سيتم حفظ المستند به"
type: docs
weight: 140
url: /ar/net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

يحصل أو يضبط الـ `PresentationFormat` الذي سيتم حفظ المستند به.

```csharp
public PresentationFormat PresentationFormat { get; set; }
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

يعرض كيفية عرض رؤية استخدام المهمة مع إعدادات مقياس الوقت المعرفة في إعدادات العرض.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// حدد SaveOptions وحدد أنه يجب استخدام إعدادات مقياس الزمن لـ TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### انظر أيضًا

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


