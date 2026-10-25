---
title: "枚举 PageSize"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.PageSize 枚举。指定页面大小。"
type: docs
weight: 3250
url: /zh/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

指定页面大小。

```csharp
public enum PageSize
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Letter | `0` | Letter 页面在点数上的尺寸为 792 × 612。 |
| Ledger | `1` | Ledger 页面在点数上的尺寸为 1224 × 792。 |
| A0 | `2` | A0 页面在点数上的尺寸为 3371 × 2384。 |
| A1 | `3` | A1 页面在点数上的尺寸为 2384 × 1685。 |
| A2 | `4` | A2 页面在点数上的尺寸为 1684 × 1190。 |
| A3 | `5` | A3 页面在点数上的尺寸为 1190 × 842。 |
| A4 | `6` | A4 页面在点数上的尺寸为 842 × 595。 |
| DefinedInView | `7` | 使用在 View 的 [`PageSettings`](../pagesettings/) 中定义的页面大小 (View.PageInfo.PageSettings)。 |

## 示例

展示如何设置一个值，指示汇总任务栏上的子任务必须向上汇总。

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // 或
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


