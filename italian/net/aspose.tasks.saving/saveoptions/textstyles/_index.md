---
title: "SaveOptions.TextStyles"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta l'elenco degli stili di testo applicati durante il rendering di una vista di progetto"
type: docs
weight: 190
url: /it/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Ottiene o imposta l'elenco degli stili di testo applicati durante il rendering di una vista di progetto.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Osservazioni

Questi stili sovrascrivono gli stili definiti in GanttCharView.TextStyles.

## Esempi

Mostra come utilizzare gli stili di testo delle opzioni di salvataggio, usati per formattare diversi elementi di testo in un progetto.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Vedi anche

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


