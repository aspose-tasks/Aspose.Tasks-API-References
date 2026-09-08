---
title: "Klasse PageInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PageInfo class. Vertegenwoordigt paginainstellingsgegevens die aanwezig zijn in MPP-bestandsformaat en worden gebruikt voor afdrukken"
type: docs
weight: 3200
url: /nl/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Stelt paginainstellingsgegevens voor die aanwezig zijn in het MPP‑bestandsformaat en worden gebruikt voor afdrukken.

```csharp
public class PageInfo
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageInfo](pageinfo/)() | Initialiseert een nieuw exemplaar van de `PageInfo` class. Vertegenwoordigt paginainstellingsgegevens die aanwezig zijn in MPP-bestandsformaat en worden gebruikt voor afdrukken. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Haalt op of stelt een exemplaar in van de [`HeaderFooterInfo`](../headerfooterinfo/) class die voettekstgegevens vertegenwoordigt. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Haalt op of stelt het exemplaar in van de [`HeaderFooterInfo`](../headerfooterinfo/) class die koptekstgegevens vertegenwoordigt. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Haalt op of stelt een exemplaar in van de [`PageLegend`](../pagelegend/) class die weergaveopties van de paginalegend specificeert. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Haalt een exemplaar op van de [`PageMargins`](../pagemargins/) class die paginamarges specificeert. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Haalt de naam op van de weergave waarvoor instellingsgegevens worden gebruikt. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Haalt een exemplaar op van de [`PageSettings`](./pagesettings/) class die afdrukinstellingen voor de pagina specificeert. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Haalt een exemplaar op van de [`PageViewSettings`](./pageviewsettings/) class die afdrukinstellingen voor de paginaview specificeert. |

## Voorbeelden

Toont hoe te werken met paginainformatie van de MS Project-weergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// laat de standaardweergave aanpassen
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// laat marges aanpassen
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// laten we paginainstellingen wijzigen
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// laten we paginaviewinstellingen wijzigen
// stel een waarde in die aangeeft of notities moeten worden afgedrukt.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// werken met project...
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


