---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "DailyCalendarRepetition-constructor. Initialiseert een nieuwe instantie van de DailyCalendarRepetition‑klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Initialiseert een nieuwe instantie van de [`DailyCalendarRepetition`](../) klasse.

```csharp
public DailyCalendarRepetition()
```

## Voorbeelden

Toont hoe te werken met dagelijkse werkherhalingspatroon‑herhalingen en een '24 uur' bij het maken van terugkerende taken.

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

// werk verder met het project...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


