---
title: "Class HeaderFooterInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.HeaderFooterInfo klasse. Vertegenwoordigt visuele inhoud van de kop- of voettekst of legende die wordt gebruikt voor afdrukken en weergave van weergaven"
type: docs
weight: 3130
url: /nl/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Stelt visuele inhoud van de kop, voettekst of legenda voor die wordt gebruikt voor afdrukken \ renderen van weergaven.

```csharp
public class HeaderFooterInfo
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Initialiseert een nieuw exemplaar van de `HeaderFooterInfo` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Haalt of stelt de gecentreerde afbeelding in die moet worden weergegeven in het bovenliggende element. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Haalt of stelt de weergegeven grootte van de centrale afbeelding in. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Haalt of stelt de gecentreerde tekst in die moet worden weergegeven in het bovenliggende element. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Krijgt of stelt de links uitgelijnde afbeelding in die moet worden weergegeven in het bovenliggende element. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Krijgt of stelt de weergegeven grootte van de linkse afbeelding in. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Krijgt of stelt de links uitgelijnde tekst in die moet worden weergegeven in het bovenliggende element. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Krijgt of stelt de rechts uitgelijnde afbeelding in die moet worden weergegeven in het bovenliggende element. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Krijgt of stelt de weergegeven grootte van de rechtse afbeelding in. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Krijgt of stelt de rechts uitgelijnde tekst in die moet worden weergegeven in het bovenliggende element. |

## Voorbeelden

Toont hoe paginakop-/voettekstinformatie gelezen kan worden.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


