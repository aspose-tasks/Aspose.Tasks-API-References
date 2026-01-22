---
title: Enum PageSize
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PageSize enum. Specifies page size
type: docs
weight: 3220
url: /net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Specifies page size.

```csharp
public enum PageSize
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Letter | `0` | The size of the Letter page in points is 792 × 612 |
| Ledger | `1` | The size of the Ledger page in points is 1224 × 792 |
| A0 | `2` | The size of the A0 page in points is 3371 × 2384 |
| A1 | `3` | The size of the A1 page in points is 2384 × 1685 |
| A2 | `4` | The size of the A2 page in points is 1684 × 1190 |
| A3 | `5` | The size of the A3 page in points is 1190 × 842 |
| A4 | `6` | The size of the A4 page in points is 842 × 595 |
| DefinedInView | `7` | Use page size defined in View's [`PageSettings`](../pagesettings/) (View.PageInfo.PageSettings). |

## Examples

Shows how to set a value indicating that subtasks on the summary task bar must be rolled up.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // OR
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


