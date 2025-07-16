---
title: Class TextStyle
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.TextStyle class. Change the visual style of the text for an item in the project view
type: docs
weight: 3340
url: /net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Change the visual style of the text for an item in the project view.

```csharp
public class TextStyle
```

## Constructors

| Name | Description |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Initializes a new instance of the `TextStyle` class with default settings. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Initializes a new instance of the `TextStyle` class with the specified font settings. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Initializes a new instance of the `TextStyle` class with the default font and specified font style. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Initializes a new instance of the `TextStyle` class with the default font and specified font size and style. |

## Properties

| Name | Description |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Gets or sets background color of the text style. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Gets or sets background pattern of the text style. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Gets or sets color of the text. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Gets or sets font of the text style. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Gets or sets [`TextItemType`](../textitemtype/) of the text style. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


