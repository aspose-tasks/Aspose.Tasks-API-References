---
title: "TextStyle.BackgroundPattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TextStyle. Ottiene o imposta il modello di sfondo dello stile di testo. BackgroundPattern"
type: docs
weight: 30
url: /it/net/aspose.tasks.visualization/textstyle/backgroundpattern/
---
## TextStyle.BackgroundPattern property

Ottiene o imposta il modello di sfondo dello stile di testo. `BackgroundPattern`.

```csharp
public BackgroundPattern BackgroundPattern { get; set; }
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

* enum [BackgroundPattern](../../../aspose.tasks/backgroundpattern/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


