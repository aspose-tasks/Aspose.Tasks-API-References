---
title: TextStyle.ItemType
second_title: Aspose.Tasks for .NET API Reference
description: TextStyle property. Gets or sets TextItemType of the text style
type: docs
weight: 60
url: /net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

Gets or sets [`TextItemType`](../../textitemtype/) of the text style.

```csharp
public virtual TextItemType ItemType { get; set; }
```

## Examples

Shows how to customize text styles which are used to style different text items in a project.

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

### See Also

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


