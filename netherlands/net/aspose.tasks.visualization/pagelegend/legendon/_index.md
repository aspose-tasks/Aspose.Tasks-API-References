---
title: "PageLegend.LegendOn"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageLegend eigenschap. Haalt de pagina's op of stelt ze in waarop de legenda verschijnt. Kan een van de waarden van de Legend-enumeratie zijn."
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

Haalt de pagina's op of stelt ze in waarop de legenda verschijnt. Kan een van de waarden van de [`Legend`](../../legend/) enumeratie zijn.

```csharp
public Legend LegendOn { get; set; }
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

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


