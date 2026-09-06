---
title: "ProjectDisplayOptions.MinuteLabel"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectDisplayOptions 属性。获取或设置分钟标签的显示方式"
type: docs
weight: 50
url: /zh/net/aspose.tasks/projectdisplayoptions/minutelabel/
---
## ProjectDisplayOptions.MinuteLabel property

获取或设置分钟标签的显示方式。

```csharp
public MinuteLabelDisplay MinuteLabel { get; set; }
```

## 示例

展示如何使用项目的显示选项。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// 设置一个值，指示当 Project 检测到手动安排的任务可能出现调度冲突时是否显示警告。
// 此选项适用于 Project 2010 及更高版本。
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// 一个值，指示是否在数字值和时间缩写前添加空格（例如 1 wk 而不是 1wk）
project.DisplayOptions.AddSpaceBeforeLabel = true;

// 设置分钟标签的显示方式
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// 设置小时标签的显示方式
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// 设置日期标签的显示方式
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// 设置周标签的显示方式
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// 设置月份标签的显示方式
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// 设置年份标签的显示方式
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// 设置一个值，指示是否在甘特图视图的顶部，以单独的汇总任务条在单行中显示整个项目的汇总信息。
project.DisplayOptions.ShowProjectSummaryTask = true;

// 设置一个值，指示当 Project 检测到手动安排的任务可能出现调度冲突时是否显示建议。
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// 设置一个值，指示是否为超链接添加下划线。
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### 另见

* enum [MinuteLabelDisplay](../../minutelabeldisplay/)
* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


