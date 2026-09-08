---
title: "PageSettings.PercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageSettings-eigenschap. Haalt een percentage van de normale grootte op of stelt deze in om het afdrukken aan te passen."
type: docs
weight: 90
url: /nl/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Haalt een percentage van de normale grootte op of stelt dit in om het afdrukken aan te passen.

```csharp
public int PercentOfNormalSize { get; set; }
```

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


