---
title: "UsageView.MiddleTimescaleTier"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "UsageView ιδιότητα. Λαμβάνει ή ορίζει τις ρυθμίσεις του μεσαίου επιπέδου κλίμακας χρόνου των προβολών. TimescaleTier"
type: docs
weight: 50
url: /el/net/aspose.tasks/usageview/middletimescaletier/
---
## UsageView.MiddleTimescaleTier property

Λαμβάνει ή ορίζει τις ρυθμίσεις του μεσαίου επιπέδου κλίμακας χρόνου της προβολής. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποδώσετε την προβολή χρήσης εργασίας με τις ρυθμίσεις χρονικής κλίμακας που ορίζονται στις ρυθμίσεις προβολής.

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

// Ορίστε τις SaveOptions και καθορίστε ότι πρέπει να χρησιμοποιηθούν οι ρυθμίσεις κλίμακας χρόνου TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Δείτε επίσης

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


