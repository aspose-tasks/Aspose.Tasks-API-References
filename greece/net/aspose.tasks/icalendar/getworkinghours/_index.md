---
title: "ICalendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ICalendar. Επιστρέφει το WorkUnit  Έναρξη, Λήξη και Διάρκεια των ωρών εργασίας για το καθορισμένο χρονικό διάστημα."
type: docs
weight: 60
url: /el/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Επιστρέφει το WorkUnit - Έναρξη, Λήξη και Διάρκεια των εργάσιμων ωρών για το καθορισμένο χρονικό διάστημα.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Ημερομηνία έναρξης του διαστήματος. |
| τελείωση | DateTime | Ημερομηνία λήξης του διαστήματος. |

### Τιμή Επιστροφής

Παράδειγμα της κλάσης [`WorkUnit`](../../workunit/) που περιέχει Έναρξη, Λήξη και Διάρκεια των ωρών εργασίας.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη μέθοδο Calendar.GetIntersectionCalendar() για να εκτελέσετε υπολογισμό στο ημερολόγιο της ανάθεσης.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### Δείτε επίσης

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Επιστρέφει την ποσότητα των εργάσιμων ωρών στην καθορισμένη ημερομηνία.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | DateTime | Η ημερομηνία για την οποία θα ληφθούν οι ώρες εργασίας. |

### Τιμή Επιστροφής

Ώρες εργασίας στην καθορισμένη ημερομηνία.

### Δείτε επίσης

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


