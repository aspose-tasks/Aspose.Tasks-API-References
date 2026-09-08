---
title: "SaveOptions.TextStyles"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt op of stelt de lijst in van tekststijlen die worden toegepast tijdens het renderen van een projectweergave."
type: docs
weight: 190
url: /nl/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Haalt op of stelt de lijst met tekststijlen in die worden toegepast tijdens het renderen van een projectweergave.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Opmerkingen

Deze stijlen overschrijven de stijlen die zijn gedefinieerd in GanttCharView.TextStyles.

## Voorbeelden

Toont hoe de tekststijlen van save options te gebruiken die worden gebruikt om verschillende tekstitems in een project te stijlen.

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

### Zie ook

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


