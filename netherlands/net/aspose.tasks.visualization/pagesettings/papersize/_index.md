---
title: "PageSettings.PaperSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageSettings-eigenschap. Haalt een papierformaat op of stelt dit in. Kan een van de waarden van de PrinterPaperSize-enumeratie zijn."
type: docs
weight: 70
url: /nl/net/aspose.tasks.visualization/pagesettings/papersize/
---
## PageSettings.PaperSize property

Haalt een papierformaat op of stelt dit in. Kan een van de waarden van de [`PrinterPaperSize`](../../printerpapersize/) enumeratie zijn.

```csharp
public PrinterPaperSize PaperSize { get; set; }
```

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

* enum [PrinterPaperSize](../../printerpapersize/)
* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


