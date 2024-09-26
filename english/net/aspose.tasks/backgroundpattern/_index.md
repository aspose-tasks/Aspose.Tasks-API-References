---
title: Enum BackgroundPattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.BackgroundPattern enum. Specifies the background pattern
type: docs
weight: 100
url: /net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Specifies the background pattern.

```csharp
public enum BackgroundPattern
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Indicates Dark diagonal left background pattern. |
| DarkDiagonalRight | `8` | Indicates Dark diagonal right background pattern. |
| DarkDither | `13` | Indicates Dark dither background pattern. |
| DarkFill | `4` | Indicates Dark fill background pattern. |
| DiagonalLeft | `5` | Indicates Diagonal left background pattern. |
| DiagonalRight | `6` | Indicates Diagonal right background pattern. |
| Hollow | `0` | Indicates Hollow background pattern. |
| LightDither | `11` | Indicates Light dither background pattern. |
| LightFill | `2` | Indicates Light fill background pattern. |
| MediumDither | `12` | Indicates Medium dither background pattern. |
| MediumFill | `3` | Indicates Medium fill background pattern. |
| MediumVerticalStripe | `10` | Indicates Medium vertical stripe background pattern. |
| SolidFill | `1` | Indicates Solid fill background pattern. |
| ThinVerticalStripe | `9` | Indicates Thin vertical stripe background pattern. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


