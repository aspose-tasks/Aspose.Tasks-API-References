---
title: "PageLegend.Width"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageLegend eigenschap. Haalt of stelt de breedte in van het linkerdeel dat standaard de projectnaam en datum bevat in de legende, in centimeters"
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

Haalt op of stelt de breedte in van het linkerdeel (standaard de projectnaam en datum bevat) van de legende in centimeters.

```csharp
public double Width { get; set; }
```

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentOutOfRangeException | Bij een poging om in te stellen op een waarde kleiner dan 0. |

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


