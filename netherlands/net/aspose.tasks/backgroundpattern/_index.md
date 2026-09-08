---
title: "Enum BackgroundPattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.BackgroundPattern enum. Specificeert het achtergrondpatroon"
type: docs
weight: 100
url: /nl/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Specificeert het achtergrondpatroon.

```csharp
public enum BackgroundPattern
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Geeft het donkere diagonale linker achtergrondpatroon aan. |
| DarkDiagonalRight | `8` | Geeft het donkere diagonale rechter achtergrondpatroon aan. |
| DarkDither | `13` | Geeft het donkere dither‑achtergrondpatroon aan. |
| DarkFill | `4` | Geeft het donkere vul‑achtergrondpatroon aan. |
| DiagonalLeft | `5` | Geeft diagonaal links achtergrondpatroon aan. |
| DiagonalRight | `6` | Geeft diagonaal rechts achtergrondpatroon aan. |
| Hollow | `0` | Geeft holle achtergrondpatroon aan. |
| LightDither | `11` | Geeft licht raster achtergrondpatroon aan. |
| LightFill | `2` | Geeft licht vul achtergrondpatroon aan. |
| MediumDither | `12` | Geeft medium raster achtergrondpatroon aan. |
| MediumFill | `3` | Geeft medium vul achtergrondpatroon aan. |
| MediumVerticalStripe | `10` | Geeft medium verticale strepen achtergrondpatroon aan. |
| SolidFill | `1` | Geeft solide vul achtergrondpatroon aan. |
| ThinVerticalStripe | `9` | Geeft dunne verticale strepen achtergrondpatroon aan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


