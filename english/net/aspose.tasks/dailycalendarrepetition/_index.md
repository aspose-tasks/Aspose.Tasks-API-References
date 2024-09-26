---
title: Class DailyCalendarRepetition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.DailyCalendarRepetition class. Represents a class for repetitions in daily recurrence pattern based on calendar days
type: docs
weight: 390
url: /net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

Represents a class for repetitions in daily recurrence pattern based on calendar days.

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | Initializes a new instance of the `DailyCalendarRepetition` class. |

## Properties

| Name | Description |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Gets or sets a number of days which represents the interval in days between occurrences. |

## Examples

Shows how to work with daily work repetition pattern repetitions and a '24 Hours' while create recurring tasks.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(calendar);
var parameters = new RecurringTaskParameters
{
    TaskName = "t1",
    Duration = project.GetDuration(1, TimeUnitType.Day),
    RecurrencePattern = new DailyRecurrencePattern
    {
        Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
        RecurrenceRange = new EndByRecurrenceRange
        {
            Start = new DateTime(2018, 7, 2, 0, 0, 0),
            Finish = new DateTime(2018, 7, 8, 16, 0, 0)
        }
    }
};
parameters.SetCalendar(project, "24 Hours");
project.RootTask.Children.Add(parameters);

// work with the project further...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


