---
title: "ProgressLines.LinePattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProgressLines 属性。获取或设置当前进度线的线型模式。LinePattern"
type: docs
weight: 110
url: /zh/net/aspose.tasks.visualization/progresslines/linepattern/
---
## ProgressLines.LinePattern property

获取或设置当前进度线的线型模式。`LinePattern`。

```csharp
public LinePattern LinePattern { get; set; }
```

## 示例

展示如何使用进度线。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// 让我们定义进度线
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// 设置显示进度线的起始日期。让我们设置项目的状态日期。
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// 设置一个值，指示是否从项目开始日期起显示进度线
progressLines.BeginAtProjectStart = true;
// 设置日期格式（<see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" />）。
progressLines.DateFormat = DateLabel.DayDddd;
// 设置一个值，指示是否在当前日期显示进度线。
progressLines.DisplayAtCurrentDate = true;
// 设置一个值，指示是否在重复间隔显示进度线。
progressLines.DisplayAtRecurringIntervals = true;
// 设置一个值，指示是否在选定日期显示进度线
progressLines.DisplaySelected = true;
// 设置一个值，指示是显示基线计划还是实际的进度线。
progressLines.IsBaselinePlan = false;
// 设置用于进度线标签的字体。
progressLines.Font = new FontDescriptor("Arial", 10);
// 设置当前进度线的颜色。
progressLines.LineColor = Color.Aquamarine;
// 设置当前进度线的线型。
progressLines.LinePattern = LinePattern.Dashed;
// 设置其他进度线的颜色。
progressLines.OtherLineColor = Color.Azure;
// 设置其他进度线的线型。
progressLines.OtherLinePattern = LinePattern.Dotted;
// 设置其他进度点的颜色。
progressLines.OtherProgressPointColor = Color.Red;
// 设置其他进度线的进度点形状。
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// 设置进度点的颜色。
progressLines.ProgressPointColor = Color.Orange;
// 设置进度点形状。
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// 设置重复间隔。
progressLines.RecurringInterval = new RecurringInterval();
// 设置重复间隔。
progressLines.RecurringInterval.Interval = Interval.Daily;
// 设置每日天数
progressLines.RecurringInterval.DailyDayNumber = 1;
// 设置一个值，指示是否为每条进度线显示日期。
progressLines.ShowDate = true;

// 让我们检查进度线
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* enum [LinePattern](../../linepattern/)
* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


