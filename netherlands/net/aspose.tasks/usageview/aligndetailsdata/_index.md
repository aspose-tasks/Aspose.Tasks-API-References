---
title: "UsageView.AlignDetailsData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "UsageView eigenschap. Haalt op of stelt de uitlijning van detailgegevens in"
type: docs
weight: 10
url: /nl/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

Krijgt of stelt de uitlijning van detailgegevens in.

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
```

## Voorbeelden

Toont hoe een taakgebruikweergave met details te renderen.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// haal de weergave op
UsageView view = (TaskUsageView)project.DefaultView;

// detailkopkolom wordt niet weergegeven
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// toon detailkopkolom
view.DisplayDetailsHeaderColumn = true;

// herhaal detailkop op alle toewijzingsrijen
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


