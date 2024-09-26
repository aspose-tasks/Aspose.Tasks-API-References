---
title: Gridline.Color
second_title: Aspose.Tasks for .NET API Reference
description: Gridline property. Gets or sets the Color of a gridline
type: docs
weight: 20
url: /net/aspose.tasks.visualization/gridline/color/
---
## Gridline.Color property

Gets or sets the `Color` of a gridline.

```csharp
public Color Color { get; set; }
```

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

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


