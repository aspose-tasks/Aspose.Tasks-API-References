---
title: "UsageView.BottomTimescaleTier"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "UsageView property. Haalt of stelt de instellingen van de onderste tijdschaal van weergaven in. TimescaleTier"
type: docs
weight: 20
url: /nl/net/aspose.tasks/usageview/bottomtimescaletier/
---
## UsageView.BottomTimescaleTier property

Haalt of stelt de instellingen van de onderste tijdschaal van de weergave in. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)

```csharp
public TimescaleTier BottomTimescaleTier { get; set; }
```

## Voorbeelden

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

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


