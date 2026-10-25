---
title: "Klasse PageLegend"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PageLegend class. Vertegenwoordigt een paginalegend die wordt gebruikt voor projectafdrukken."
type: docs
weight: 3210
url: /nl/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Stelt een paginalegende voor die wordt gebruikt voor projectafdrukken.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageLegend](pagelegend/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Haalt of stelt de gecentreerde afbeelding in die moet worden weergegeven in het bovenliggende element. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Haalt of stelt de weergegeven grootte van de centrale afbeelding in. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Haalt of stelt de gecentreerde tekst in die moet worden weergegeven in het bovenliggende element. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Krijgt of stelt de links uitgelijnde afbeelding in die moet worden weergegeven in het bovenliggende element. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Krijgt of stelt de weergegeven grootte van de linkse afbeelding in. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Krijgt of stelt de links uitgelijnde tekst in die moet worden weergegeven in het bovenliggende element. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Haalt op of stelt de pagina's in waarop de legende verschijnt. Kan een van de waarden van de [`Legend`](../legend/) enumeratie zijn. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Krijgt of stelt de rechts uitgelijnde afbeelding in die moet worden weergegeven in het bovenliggende element. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Krijgt of stelt de weergegeven grootte van de rechtse afbeelding in. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Krijgt of stelt de rechts uitgelijnde tekst in die moet worden weergegeven in het bovenliggende element. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Haalt op of stelt de breedte in van het linkerdeel (standaard de projectnaam en datum bevat) van de legende in centimeters. |

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

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


