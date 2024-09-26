---
title: PageLegend.RightImage
second_title: Aspose.Tasks for .NET API Reference
description: PageLegend property. Gets or sets the right aligned image to be displayed in the page legend
type: docs
weight: 70
url: /net/aspose.tasks.visualization/pagelegend/rightimage/
---
## PageLegend.RightImage property

Gets or sets the right aligned image to be displayed in the page legend.

```csharp
public Image RightImage { get; set; }
```

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


