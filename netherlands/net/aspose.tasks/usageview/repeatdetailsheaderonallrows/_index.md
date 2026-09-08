---
title: "UsageView.RepeatDetailsHeaderOnAllRows"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "UsageView property. Haalt of stelt een waarde in die aangeeft of de detailkop op elke toewijzingsrij moet worden herhaald of niet"
type: docs
weight: 60
url: /nl/net/aspose.tasks/usageview/repeatdetailsheaderonallrows/
---
## UsageView.RepeatDetailsHeaderOnAllRows property

Haalt op of stelt een waarde in die aangeeft of de detailkop op alle toewijzingsrijen moet worden herhaald of niet.

```csharp
public bool RepeatDetailsHeaderOnAllRows { get; set; }
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


