---
title: "Calendar.GetIntersectionCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Λαμβάνει το αντικείμενο ICalendar που μπορεί να χρησιμοποιηθεί για εκτέλεση υπολογισμών στην τομή των προγραμμάτων εργασίας των 2 ημερολογίων"
type: docs
weight: 280
url: /el/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Λαμβάνει το αντικείμενο [`ICalendar`](../../icalendar/) που μπορεί να χρησιμοποιηθεί για εκτέλεση υπολογισμών στην τομή των προγραμμάτων εργασίας των 2 ημερολογίων.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| calendar1 | Calendar | Πρώτο ημερολόγιο. |
| calendar2 | Calendar | Δεύτερο ημερολόγιο. |

### Τιμή Επιστροφής

Υλοποίηση της διεπαφής ICalendar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | Όταν κάποιο από τα ορίσματα είναι null. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


