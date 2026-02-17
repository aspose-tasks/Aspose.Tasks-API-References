---
title: Class Gridlines
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.Gridlines class. Represents gridlines that appear in a GanttChart view
type: docs
weight: 3100
url: /net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Represents gridlines that appear in a GanttChart view.

```csharp
public class Gridlines
```

## Constructors

| Name | Description |
| --- | --- |
| [Gridlines](gridlines/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Gets or sets the number from 0 to 99 that specifies the interval between gridlines. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Gets or sets the color of secondary gridlines. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Gets or sets the line pattern for secondary gridlines. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Gets or sets the color of normal gridlines. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Gets or sets the line pattern for normal gridlines. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Gets or sets the gridline type. |

## Examples

Shows how to work with gridlines.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// lets tune the first gridline of the view
var gridlines = view.Gridlines[0];
// set the number from 0 to 99 that specifies the interval between gridlines.
gridlines.Interval = 2;
// set the color of secondary gridlines.
gridlines.IntervalColor = Color.Red;
// set the line pattern for secondary gridlines
gridlines.IntervalPattern = LinePattern.Solid;
// set the color of normal gridlines
gridlines.NormalColor = Color.Blue;
// set the line pattern for normal gridlines
gridlines.NormalPattern = LinePattern.CloseDot;
// set the gridline type
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


