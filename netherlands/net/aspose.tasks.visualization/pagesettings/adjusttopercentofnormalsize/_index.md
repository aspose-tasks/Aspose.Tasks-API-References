---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageSettings-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of het afdrukken moet worden aangepast aan het opgegeven percentage PercentOfNormalSize van de normale grootte."
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

Haalt een waarde op of stelt deze in die aangeeft of het afdrukken moet worden aangepast aan het opgegeven percentage ([`PercentOfNormalSize`](../percentofnormalsize/)) van de normale grootte.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## Opmerkingen

Is niet effectief wanneer het project wordt gerenderd in HTML-indeling.

## Voorbeelden

Toont hoe een weergave te renderen met de opgegeven schaalfactor.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// stel een waarde in die aangeeft dat de weergave geschaald moet worden met de opgegeven schaalfactor
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// specificeer de schaalfactor
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Zie ook

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


