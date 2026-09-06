---
title: "GanttBarSize 枚举"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GanttBarSize 枚举。指定条形的高度（单位为点）"
type: docs
weight: 700
url: /zh/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

指定条形的高度（单位为点）。

```csharp
public enum GanttBarSize
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| BarSize6 | `0` | 条形大小为 6 点。 |
| BarSize8 | `1` | 条形大小为 8 点。 |
| BarSize10 | `2` | 条形大小 10 点。 |
| BarSize12 | `3` | 条形大小 12 点。 |
| BarSize14 | `4` | 条形大小 14 点。 |
| BarSize18 | `5` | 条形大小 18 点。 |
| BarSize24 | `6` | 条形大小 24 点。 |

## 示例

展示如何设置甘特图视图的一些有用属性。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// 设置一个值，指示条形是否四舍五入到最近的一天
view.BarRounding = false;
// 设置甘特图中甘特条的高度（单位为点）
view.BarSize = GanttBarSize.BarSize24;
// 设置一个值，指示在展开汇总任务时是否隐藏汇总条
view.HideRollupBarsWhenSummaryExpanded = true;
// 设置非工作时间颜色
view.NonWorkingTimeColor = Color.Azure;
// 设置一个值，指示甘特图上的条形是否必须汇总
view.RollUpGanttBars = true;
// 设置一个值，指示甘特图上的任务拆分是否必须显示
view.ShowBarSplits = true;
// 设置一个值，指示甘特图上的绘图是否必须显示
view.ShowDrawings = true;
// 设置一个百分比，以缩小或放大时间刻度层级上单位之间的间距
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


