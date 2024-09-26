---
title: ProjectDisplayOptions.ShowProjectSummaryTask
second_title: Aspose.Tasks for .NET API Reference
description: ProjectDisplayOptions property. Gets or sets a value indicating whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view
type: docs
weight: 70
url: /net/aspose.tasks/projectdisplayoptions/showprojectsummarytask/
---
## ProjectDisplayOptions.ShowProjectSummaryTask property

Gets or sets a value indicating whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view.

```csharp
public bool ShowProjectSummaryTask { get; set; }
```

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

* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


