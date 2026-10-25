---
title: "TextStyle.Color"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TextStyle. Ottiene o imposta il colore del testo"
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/textstyle/color/
---
## TextStyle.Color property

Ottiene o imposta il colore del testo.

```csharp
public Color Color { get; set; }
```

## Esempi

Mostra come personalizzare gli stili di testo che vengono usati per formattare diversi elementi di testo in un progetto.

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

### Vedi anche

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


