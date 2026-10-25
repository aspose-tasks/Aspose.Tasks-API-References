---
title: "Κλάση DailyCalendarRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.DailyCalendarRepetition. Αντιπροσωπεύει μια κλάση για επαναλήψεις σε ημερήσιο μοτίβο επανάληψης βασισμένο σε ημερολογιακές ημέρες"
type: docs
weight: 390
url: /el/net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

Αντιπροσωπεύει μια κλάση για επαναλήψεις σε καθημερινό μοτίβο επανάληψης βασισμένο σε ημερολογιακές ημέρες.

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `DailyCalendarRepetition`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Λαμβάνει ή ορίζει έναν αριθμό ημερών που αντιπροσωπεύει το διάστημα σε ημέρες μεταξύ των εμφανίσεων. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


