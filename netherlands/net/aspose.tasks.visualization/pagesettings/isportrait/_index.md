---
title: "PageSettings.IsPortrait"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageSettings-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is."
type: docs
weight: 40
url: /nl/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Haalt op of stelt een waarde in die aangeeft of de paginarichting portret is; geeft onwaar terug als de paginarichting landschap is.

```csharp
public bool IsPortrait { get; set; }
```

## Opmerkingen

Is van toepassing tijdens het renderen wanneer SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

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

Toont hoe de paginagrootte en -oriëntatie te specificeren met behulp van View-instellingen of SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// In dit geval worden de paginagrootte en -oriëntatie toegepast vanuit de eigenschappen view.PageInfo.PageSettings.PaperSize en view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// In dit geval worden de paginagrootte en -oriëntatie toegepast vanuit de eigenschappen van SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// In dit geval wordt de paginagrootte toegepast vanuit SaveOptions.CustomPageSize. De IsPortrait-eigenschap wordt niet in aanmerking genomen.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Zie ook

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


