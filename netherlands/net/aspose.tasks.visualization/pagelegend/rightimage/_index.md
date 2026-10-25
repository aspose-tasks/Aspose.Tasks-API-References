---
title: "PageLegend.RightImage"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageLegend eigenschap. Haalt of stelt de rechts uitgelijnde afbeelding in die in de paginale legende wordt weergegeven"
type: docs
weight: 70
url: /nl/net/aspose.tasks.visualization/pagelegend/rightimage/
---
## PageLegend.RightImage property

Haalt of stelt de rechts uitgelijnde afbeelding in die in de paginale legende wordt weergegeven.

```csharp
public Image RightImage { get; set; }
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


