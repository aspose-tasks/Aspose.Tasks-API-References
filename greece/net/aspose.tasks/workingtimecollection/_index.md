---
title: "Κλάση WorkingTimeCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WorkingTimeCollection κλάση. Αναπαριστά μια συλλογή αντικειμένων WorkingTimeCollection"
type: docs
weight: 3670
url: /el/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Αναπαριστά μια συλλογή αντικειμένων `WorkingTimeCollection`.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `WorkingTimeCollection`. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Προσθέτει μια νέα παρουσία WorkingTime σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Αφαιρεί όλα τα στοιχεία [`WorkingTime`](../workingtime/) από τη συλλογή. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Ελέγχει αν το καθορισμένο στοιχείο βρίσκεται στη Λίστα. Εκτελεί μια γραμμική αναζήτηση O(n). |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | αντιγράφει το περιεχόμενο μιας συλλογής σε έναν Πίνακα, ξεκινώντας από ένα συγκεκριμένο δείκτη |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Αφαιρεί την παρουσία [`WorkingTime`](../workingtime/) από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Μετατρέπει το αντικείμενο WorkingTimeCollection σε λίστα αντικειμένων [`WorkingTime`](../workingtime/). |

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

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


