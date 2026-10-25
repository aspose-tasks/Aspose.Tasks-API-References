---
title: "Klasse TextStyle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.TextStyle class. Wijzig de visuele stijl van de tekst voor een item in de projectweergave"
type: docs
weight: 3420
url: /nl/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Wijzig de visuele stijl van de tekst voor een item in de projectweergave.

```csharp
public class TextStyle
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Initialiseert een nieuw exemplaar van de `TextStyle`-klasse met standaardinstellingen. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Initialiseert een nieuw exemplaar van de `TextStyle`-klasse met de opgegeven lettertype-instellingen. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Initialiseert een nieuw exemplaar van de `TextStyle`-klasse met het standaardlettertype en de opgegeven lettertype-stijl. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Initialiseert een nieuw exemplaar van de `TextStyle`-klasse met het standaardlettertype en de opgegeven lettertypegrootte en -stijl. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Haalt op of stelt de achtergrondkleur van de tekststijl in. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Haalt op of stelt het achtergrondpatroon van de tekststijl in. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Haalt op of stelt de kleur van de tekst in. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Haalt op of stelt het lettertype van de tekststijl in. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Haalt op of stelt [`TextItemType`](../textitemtype/) van de tekststijl in. |

## Voorbeelden

Toont hoe tekststijlen aan te passen die worden gebruikt om verschillende tekstitems in een project op te maken.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


