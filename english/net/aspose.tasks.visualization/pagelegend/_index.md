---
title: Class PageLegend
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PageLegend class. Represents a page legend which is used for project printing
type: docs
weight: 3190
url: /net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Represents a page legend which is used for project printing.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Constructors

| Name | Description |
| --- | --- |
| [PageLegend](pagelegend/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Gets or sets the centered image to be displayed in the parent element. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Gets or sets the displayed size of the center image. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Gets or sets the centered text to display in the parent element. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Gets or sets the left aligned image to be displayed in the parent element. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Gets or sets the displayed size of the left image. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Gets or sets the left aligned text to display in the parent element. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Gets or sets the pages on which the legend appears. Can be one of the values of the [`Legend`](../legend/) enumeration. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Gets or sets the right aligned image to be displayed in the parent element. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Gets or sets the displayed size of the right image. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Gets or sets the right aligned text to display in the parent element. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Gets or sets the width of the left part (containing project's name and date by default) of the legend in centimeters. |

## Examples

Shows how to work with page legend information.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// lets read page legend information
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// also modification of a legend is supported
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


