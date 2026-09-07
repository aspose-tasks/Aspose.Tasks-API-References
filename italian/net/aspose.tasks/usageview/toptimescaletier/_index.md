---
title: "UsageView.TopTimescaleTier"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "proprietà UsageView. Ottiene o imposta le impostazioni del tier di scala temporale superiore delle visualizzazioni. TimescaleTier"
type: docs
weight: 80
url: /it/net/aspose.tasks/usageview/toptimescaletier/
---
## UsageView.TopTimescaleTier property

Ottiene o imposta le impostazioni del tier di scala temporale superiore della visualizzazione. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## Esempi

Mostra come renderizzare la visualizzazione dell'utilizzo delle attività con le impostazioni della scala temporale definite nelle impostazioni della vista.

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

// Definisci le SaveOptions e specifica che le impostazioni della scala temporale TaskUsageView devono essere utilizzate.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Vedi anche

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


