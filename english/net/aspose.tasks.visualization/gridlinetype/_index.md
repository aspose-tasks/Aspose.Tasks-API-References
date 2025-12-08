---
title: Enum GridlineType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.GridlineType enum. Type of gridline
type: docs
weight: 3060
url: /net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Type of gridline.

```csharp
public enum GridlineType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| GanttRow | `0` | Indicates Gridline of a gantt row grid line type. |
| TopTierColumn | `1` | Indicates Gridline of top tier column grid line type. |
| BottomTierColumn | `2` | Indicates Gridline of bottom tier column grid line type. |
| SheetRow | `3` | Indicates Gridline of a sheet row grid line type. |
| SheetColumn | `4` | Indicates Gridline of a sheet column grid line type. |
| UsageRow | `5` | Indicates Gridline of a usage row grid line type. |
| UsageColumn | `6` | Indicates Gridline of a usage column grid line type. |
| GanttTitleVertical | `7` | Indicates Gantt title vertical grid line type. |
| GanttTitleHorizontal | `8` | Indicates Gantt title horizontal grid line type. |
| BarRows | `9` | Indicates Bar rows grid line type. |
| GanttProjectStart | `10` | Indicates Gantt project start grid line type. |
| GanttProjectFinish | `11` | Indicates Gantt project finish grid line type. |
| GanttStatusDate | `12` | Indicates Gantt status date grid line type. |
| GanttCurrentDate | `13` | Indicates Gantt current date grid line type. |
| GanttPageBreaks | `14` | Indicates Gantt page breaks grid line type. |
| MiddleTierColumn | `15` | Indicates Gridline of middle tier column grid line type. |

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


