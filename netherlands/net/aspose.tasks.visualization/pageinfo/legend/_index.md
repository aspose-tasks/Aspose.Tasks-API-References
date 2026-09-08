---
title: "PageInfo.Legend"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageInfo eigenschap. Haalt op of stelt een instantie in van de PageLegend-klasse die weergaveopties van de paginalegend specificeert."
type: docs
weight: 40
url: /nl/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

Haalt op of stelt een instantie in van de [`PageLegend`](../../pagelegend/) klasse die weergaveoptjes van de paginalegend specificeert.

```csharp
public PageLegend Legend { get; set; }
```

## Opmerkingen

Momenteel is dit alleen van toepassing op Gantt-diagramweergaven.

## Voorbeelden

Toont hoe te werken met paginalegendinformatie.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// laten we paginalegendinformatie lezen
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// ook wijziging van een legende wordt ondersteund
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

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

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


