---
title: DailyCalendarRepetition.DailyCalendarRepetition
second_title: Aspose.Tasks for .NET API Reference
description: DailyCalendarRepetition constructor. Initializes a new instance of the DailyCalendarRepetition class
type: docs
weight: 10
url: /net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Initializes a new instance of the [`DailyCalendarRepetition`](../) class.

```csharp
public DailyCalendarRepetition()
```

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

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


