---
title: "PageLegend.CenteredText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageLegend eigenschap. Haalt de gecentreerde tekst op of stelt deze in die moet worden weergegeven in de paginalegenda."
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/pagelegend/centeredtext/
---
## PageLegend.CenteredText property

Haalt de gecentreerde tekst op of stelt deze in die moet worden weergegeven in de paginalegenda.

```csharp
public string CenteredText { get; set; }
```

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

### Zie ook

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


