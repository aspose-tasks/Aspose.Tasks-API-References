---
title: "Klasse PageViewSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PageViewSettings klasse. Vertegenwoordigt afdrukinstellingen voor een projectweergave"
type: docs
weight: 3260
url: /nl/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Stelt afdrukinstellingen voor een projectweergave voor.

```csharp
public class PageViewSettings
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Haalt op of stelt het aantal eerste kolommen in dat op alle pagina's moet worden afgedrukt. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de tijdschaal moet worden aangepast aan het einde van een pagina bij het afdrukken. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of alle bladkolommen van een weergave moeten worden afgedrukt. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of lege pagina's van een weergave moeten worden afgedrukt. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een opgegeven aantal eerste kolommen op alle pagina's moeten worden afgedrukt. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of notities moeten worden afgedrukt. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


