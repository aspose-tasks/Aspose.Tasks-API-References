---
title: "SaveOptions.PresentationFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Belgenin kaydedileceği PresentationFormat'ı alır veya ayarlar."
type: docs
weight: 140
url: /tr/net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

Belgenin kaydedileceği `PresentationFormat`'ı alır veya ayarlar.

```csharp
public PresentationFormat PresentationFormat { get; set; }
```

## Örnekler

Özet görev çubuğundaki alt görevlerin toplanması gerektiğini gösteren bir değerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // VEYA
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

Görünüm ayarlarında tanımlanan zaman ölçeği ayarlarıyla görev kullanım görünümünün nasıl oluşturulacağını gösterir.

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

// SaveOptions'ı tanımlayın ve TaskUsageView zaman ölçeği ayarlarının kullanılmasını belirtin.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Ayrıca Bakınız

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


