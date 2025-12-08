---
title: Class Gridline
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.Gridline class. The horizontal or vertical line that appears in the project view
type: docs
weight: 3050
url: /net/aspose.tasks.visualization/gridline/
---
## Gridline class

The horizontal or vertical line that appears in the project view.

```csharp
public class Gridline
```

## Constructors

| Name | Description |
| --- | --- |
| [Gridline](gridline/)() | Initializes a new instance of the `Gridline` class. |

## Properties

| Name | Description |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Gets or sets the [`Color`](./color/) of a gridline. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Gets or sets the type of gridline ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Gets or sets the [`LinePattern`](../linepattern/) of a gridline. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Returns a flag indicating whether this instance is equal to the specified object. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Returns a hash code value for the instance of the `Gridline` class. |

## Examples

Shows how to work with gridlines while save in visual formats.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // set the type of gridline (<see cref="P:Aspose.Tasks.Visualization.Gridline.GridlineType" />).
    GridlineType = GridlineType.GanttRow, 
    // set the <see cref="T:Aspose.Tasks.Visualization.LinePattern" /> of a gridline
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


