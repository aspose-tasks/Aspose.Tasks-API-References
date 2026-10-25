---
title: "PageViewSettings.PrintNotes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageViewSettings-eigenschap. Geeft of stelt een waarde in die aangeeft of notities moeten worden afgedrukt"
type: docs
weight: 70
url: /nl/net/aspose.tasks.visualization/pageviewsettings/printnotes/
---
## PageViewSettings.PrintNotes property

Haalt op of stelt een waarde in die aangeeft of notities moeten worden afgedrukt.

```csharp
public bool PrintNotes { get; set; }
```

## Voorbeelden

Toont hoe taak-, resource- en toewijzingsnotities op een aparte pagina kunnen worden afgedrukt.

```csharp
var project = new Project(DataDir + "Input.mpp");

// stel het aantal eerste kolommen in dat op alle pagina's moet worden afgedrukt
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// stel een waarde in die aangeeft of notities moeten worden afgedrukt.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// stel een waarde in die aangeeft of de tijdschaal moet worden aangepast aan het einde van een pagina bij het afdrukken.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// stel een waarde in die aangeeft of alle bladkolommen van een weergave moeten worden afgedrukt
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// stel een waarde in die aangeeft of lege pagina's van een weergave moeten worden afgedrukt
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// stel een waarde in die aangeeft of een opgegeven aantal eerste kolommen op alle pagina's moet worden afgedrukt
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


