---
title: "PageSettings.PagesInHeight"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageSettings-eigenschap. Haalt een aantal pagina's in hoogte op of stelt dit in die moeten worden afgedrukt."
type: docs
weight: 50
url: /nl/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

Haalt een aantal pagina's in hoogte op of stelt dit in voor afdrukken.

```csharp
public int PagesInHeight { get; set; }
```

## Voorbeelden

Toont hoe een weergave te renderen met de optie 'Fit X aan Y pagina\'s' .

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// specificeer dat de weergave in 2 pagina's of minder in hoogte moet worden gerenderd
view.PageInfo.PageSettings.PagesInHeight = 2;
// specificeer dat de weergave in 1 pagina in breedte moet worden gerenderd
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### Zie ook

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


