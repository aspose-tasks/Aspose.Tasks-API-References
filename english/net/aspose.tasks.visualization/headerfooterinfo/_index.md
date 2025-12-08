---
title: Class HeaderFooterInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.HeaderFooterInfo class. Represents visual content of the header footer or legend which is used for printing  rendering of views
type: docs
weight: 3080
url: /net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Represents visual content of the header, footer or legend which is used for printing \ rendering of views.

```csharp
public class HeaderFooterInfo
```

## Constructors

| Name | Description |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Initializes a new instance of the `HeaderFooterInfo` class. |

## Properties

| Name | Description |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Gets or sets the centered image to be displayed in the parent element. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Gets or sets the displayed size of the center image. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Gets or sets the centered text to display in the parent element. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Gets or sets the left aligned image to be displayed in the parent element. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Gets or sets the displayed size of the left image. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Gets or sets the left aligned text to display in the parent element. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Gets or sets the right aligned image to be displayed in the parent element. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Gets or sets the displayed size of the right image. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Gets or sets the right aligned text to display in the parent element. |

## Examples

Shows how to read page header/footer info.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


