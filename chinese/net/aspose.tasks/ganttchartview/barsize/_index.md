---
title: "GanttChartView.BarSize"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttChartView 属性。获取或设置 Gantt Chart 中甘特条的高度（以点为单位）"
type: docs
weight: 40
url: /zh/net/aspose.tasks/ganttchartview/barsize/
---
## GanttChartView.BarSize property

获取或设置甘特图中甘特条的高度（单位：点）。

```csharp
public GanttBarSize BarSize { get; set; }
```

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

* enum [GanttBarSize](../../ganttbarsize/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


