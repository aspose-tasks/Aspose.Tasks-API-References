---
title: RecurringInterval.DailyWorkday
second_title: Aspose.Tasks for .NET API Reference
description: RecurringInterval property. Gets or sets a value indicating whether a day is workday for daily progress lines
type: docs
weight: 30
url: /net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

Gets or sets a value indicating whether a day is workday for daily progress lines.

```csharp
public bool DailyWorkday { get; set; }
```

## Examples

Shows how to add daily recurring interval of progress lines.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// set the daily pattern day number
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// set a value indicating whether a day is workday for daily progress lines.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### See Also

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


