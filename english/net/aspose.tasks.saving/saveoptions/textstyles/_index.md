---
title: SaveOptions.TextStyles
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets the list of text styles that applied during rendering of a project view
type: docs
weight: 190
url: /net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Gets or sets the list of text styles that applied during rendering of a project view.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Remarks

These styles override styles defined in GanttCharView.TextStyles.

## Examples

Shows how to use save options' text styles which are used to style different text items in a project.

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

### See Also

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


