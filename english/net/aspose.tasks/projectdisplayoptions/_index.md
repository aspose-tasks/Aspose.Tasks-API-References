---
title: Class ProjectDisplayOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProjectDisplayOptions class. Represents the display options for a project instance
type: docs
weight: 1420
url: /net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Represents the display options for a project instance.

```csharp
public class ProjectDisplayOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Initializes a new instance of the `ProjectDisplayOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Gets or sets a value indicating whether to add a space before the number value and the time abbreviation (1 wk as opposed to 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Gets or sets how the day label displays. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Gets or sets how the hour label displays. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Gets or sets how the minute label displays. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Gets or sets how the month label displays. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Gets or sets a value indicating whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Gets or sets a value indicating whether to show suggestions when Project identifies a possible scheduling conflict with a manually scheduled task. This option is available for Project 2010 version and later. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Gets or sets a value indicating whether to show warnings when Project identifies a possible scheduling conflict with a manually scheduled task. This option is available for Project 2010 version and later. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Gets or sets a value indicating whether to underline hyperlinks. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Gets or sets how the week label displays. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Gets or sets how the year label displays. |

## Examples

Shows how to use project's display options.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Set a value indicating whether to show warnings when Project identifies a possible scheduling conflict with a manually scheduled task.
// This option is available for Project 2010 version and later.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// a value indicating whether to add a space before the number value and the time abbreviation (1 wk as opposed to 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// set how the minute label is displayed
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// set how the hour label is displayed
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// set how the day label is displayed
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// set how the week label is displayed
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// set how the month label is displayed
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// set how the year label is displayed
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// set a value indicating whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view.
project.DisplayOptions.ShowProjectSummaryTask = true;

// set a value indicating whether to show suggestions when Project identifies a possible scheduling conflict with a manually scheduled task.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// set a value indicating whether to underline hyperlinks.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


