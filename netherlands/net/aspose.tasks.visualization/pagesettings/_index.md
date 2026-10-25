---
title: "Klasse PageSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PageSettings klasse. Vertegenwoordigt afdrukinstellingen voor een pagina van de projectweergave"
type: docs
weight: 3240
url: /nl/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Stelt afdrukinstellingen voor een pagina van de projectweergave voor.

```csharp
public class PageSettings
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageSettings](pagesettings/)() | Initialiseert een nieuw exemplaar van de `PageSettings` klasse. Vertegenwoordigt afdrukinstellingen voor een pagina van de projectweergave. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of het afdrukken moet worden aangepast naar het opgegeven percentage ([`PercentOfNormalSize`](./percentofnormalsize/)) van de normale grootte. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Haalt een eerste paginanummer op of stelt deze in voor afdrukken. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de paginarichting portret is; geeft onwaar terug als de paginarichting landschap is. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Haalt een aantal pagina's in hoogte op of stelt dit in voor afdrukken. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Haalt een aantal pagina's in breedte op of stelt dit in voor afdrukken. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Haalt een papierformaat op of stelt dit in. Kan een van de waarden van de enumeratie [`PrinterPaperSize`](../printerpapersize/) zijn. |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Haalt een geheel getal op of stelt dit in dat een van de PrinterPaperSize-waarden of een aangepast paginagrootte‑id vertegenwoordigt. Deze waarde kan worden gebruikt om PaperSize op te halen uit de OS‑instellingen. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Haalt een percentage van de normale grootte op of stelt dit in om het afdrukken aan te passen. |

## Voorbeelden

Toont hoe te werken met &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// haal de instellingen op
var settings = project.DefaultView.PageInfo.PageSettings;
// laten we enkele eigenschappen afstemmen
// stelt een waarde in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is.
settings.IsPortrait = true;
// stelt een aantal pagina's in breedte in om af te drukken.
settings.PagesInWidth = 5;
// stelt een aantal pagina's in hoogte in om af te drukken.
settings.PagesInHeight = 7;
// stelt een percentage van de normale grootte in om het afdrukken aan te passen.
settings.PercentOfNormalSize = 200;
// stelt een papierformaat in. Kan een van de waarden van de enumeratie <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" /> zijn.
settings.PaperSize = PrinterPaperSize.PaperB4;
// stelt een eerste paginanummer in voor afdrukken.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


