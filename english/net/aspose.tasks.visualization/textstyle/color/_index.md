---
title: TextStyle.Color
second_title: Aspose.Tasks for .NET API Reference
description: TextStyle property. Gets or sets color of the text
type: docs
weight: 40
url: /net/aspose.tasks.visualization/textstyle/color/
---
## TextStyle.Color property

Gets or sets color of the text.

```csharp
public Color Color { get; set; }
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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


