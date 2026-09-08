---
title: "PageInfo.Header"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageInfo eigenschap. Haalt op of stelt de instantie in van de HeaderFooterInfo-klasse die headergegevens vertegenwoordigt."
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/pageinfo/header/
---
## PageInfo.Header property

Haalt op of stelt de instantie in van de [`HeaderFooterInfo`](../../headerfooterinfo/) klasse die headergegevens vertegenwoordigt.

```csharp
public HeaderFooterInfo Header { get; set; }
```

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

* class [HeaderFooterInfo](../../headerfooterinfo/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


