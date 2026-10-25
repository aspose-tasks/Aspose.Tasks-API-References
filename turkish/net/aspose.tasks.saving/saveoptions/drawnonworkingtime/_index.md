---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Çalışma dışı zamanın çizilip çizilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer TRUE'dır."
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri alır veya ayarlar (Varsayılan değer TRUE'dır).

```csharp
public bool DrawNonWorkingTime { get; set; }
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

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


