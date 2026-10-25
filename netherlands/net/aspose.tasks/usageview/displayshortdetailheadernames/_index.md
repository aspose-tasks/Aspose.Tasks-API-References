---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "UsageView eigenschap. Haalt op of stelt een waarde in die aangeeft of korte detailkopnamen moeten worden weergegeven of niet"
type: docs
weight: 40
url: /nl/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

Haalt op of stelt een waarde in die aangeeft of korte detailkopnamen al dan niet worden weergegeven.

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
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

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


