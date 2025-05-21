---
title: PageLegend.Width
second_title: Aspose.Tasks for .NET API Reference
description: PageLegend property. Gets or sets the width of the left part containing projects name and date by default of the legend in centimeters
type: docs
weight: 30
url: /net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

Gets or sets the width of the left part (containing project's name and date by default) of the legend in centimeters.

```csharp
public double Width { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | When attempting to set to a value less than 0. |

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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


