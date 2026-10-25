---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "DailyCalendarRepetition κατασκευαστής. Αρχικοποιεί μια νέα παρουσία της κλάσης DailyCalendarRepetition"
type: docs
weight: 10
url: /el/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`DailyCalendarRepetition`](../).

```csharp
public DailyCalendarRepetition()
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με επαναλήψεις προτύπου ημερήσιας εργασίας και ένα '24 Hours' κατά τη δημιουργία επαναλαμβανόμενων εργασιών.

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

// συνεχίστε την εργασία με το έργο...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


