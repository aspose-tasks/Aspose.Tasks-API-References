---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of niet-werkelijke tijd moet worden getekend. Standaardwaarde is TRUE."
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Haalt op of stelt een waarde in die aangeeft of niet-werkelijke tijd moet worden getekend (Standaardwaarde is WAAR).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

## Voorbeelden

Toont hoe een waarde in te stellen die aangeeft dat subtaken op de samenvattingstaakbalk moeten worden opgeteld.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // OF
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Zie ook

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


