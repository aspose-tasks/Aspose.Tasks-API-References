---
title: "SaveOptions.PresentationFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt het PresentationFormat op of stelt dit in waarin het document wordt opgeslagen"
type: docs
weight: 140
url: /nl/net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

Haalt het `PresentationFormat` op of stelt dit in waarin het document wordt opgeslagen.

```csharp
public PresentationFormat PresentationFormat { get; set; }
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

Toont hoe de taakgebruikweergave te renderen met tijdschaalinstellingen gedefinieerd in de weergave-instellingen.

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

// Definieer de SaveOptions en specificeer dat de tijdschaalinstellingen van TaskUsageView moeten worden gebruikt.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Zie ook

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


