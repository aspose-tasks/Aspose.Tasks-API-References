---
title: "WorkingTimeCollection.Add"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος WorkingTimeCollection. Προσθέτει μια νέα παρουσία WorkingTime σε αυτή τη συλλογή"
type: docs
weight: 30
url: /el/net/aspose.tasks/workingtimecollection/add/
---
## WorkingTimeCollection.Add method

Προσθέτει μια νέα παρουσία WorkingTime σε αυτή τη συλλογή.

```csharp
public bool Add(WorkingTime item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | WorkingTime | Το στοιχείο προς προσθήκη. |

### Τιμή Επιστροφής

αληθές εάν το αντικείμενο WorkingTime έχει προστεθεί επιτυχώς· διαφορετικά, ψευδές.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη συλλογή χρόνου εργασίας.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// εκτυπώστε τις ώρες εργασίας του Σαββάτου
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// εκτυπώστε τις ώρες εργασίας της Κυριακής
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Μπορείτε περαιτέρω να διασχίσετε τους χρόνους εργασίας και να τους εμφανίσετε.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### Δείτε επίσης

* class [WorkingTime](../../workingtime/)
* class [WorkingTimeCollection](../)
* namespace [Aspose.Tasks](../../workingtimecollection/)
* assembly [Aspose.Tasks](../../../)


