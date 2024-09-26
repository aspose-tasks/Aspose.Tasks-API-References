---
title: Gridlines.IntervalPattern
second_title: Aspose.Tasks for .NET API Reference
description: Gridlines property. Gets or sets the line pattern for secondary gridlines
type: docs
weight: 40
url: /net/aspose.tasks.visualization/gridlines/intervalpattern/
---
## Gridlines.IntervalPattern property

Gets or sets the line pattern for secondary gridlines.

```csharp
public LinePattern IntervalPattern { get; set; }
```

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

* enum [LinePattern](../../linepattern/)
* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


