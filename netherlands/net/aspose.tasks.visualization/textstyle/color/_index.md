---
title: "TextStyle.Color"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TextStyle-eigenschap. Haalt of stelt de kleur van de tekst in"
type: docs
weight: 40
url: /nl/net/aspose.tasks.visualization/textstyle/color/
---
## TextStyle.Color property

Haalt op of stelt de kleur van de tekst in.

```csharp
public Color Color { get; set; }
```

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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


