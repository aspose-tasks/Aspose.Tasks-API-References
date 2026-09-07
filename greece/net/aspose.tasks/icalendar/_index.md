---
title: "Διεπαφή ICalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Διεπαφή Aspose.Tasks.ICalendar. Αντιπροσωπεύει μια αφηρημένη αναπαράσταση ημερολογίου που μπορεί να χρησιμοποιηθεί για διάφορους υπολογισμούς ημερομηνιών και διάρκειων."
type: docs
weight: 840
url: /el/net/aspose.tasks/icalendar/
---
## ICalendar interface

Αναπαριστά μια αφηρημένη αναπαράσταση ημερολογίου που μπορεί να χρησιμοποιηθεί για διάφορους υπολογισμούς ημερομηνιών και διάρκειων.

```csharp
public interface ICalendar
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας για την καθορισμένη ημερομηνία. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από την ημερομηνία έναρξής της, τα διαχωρισμένα μέρη και τη διάρκεια εργασίας. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Επιστρέφει την ποσότητα των εργάσιμων ωρών στην καθορισμένη ημερομηνία. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Επιστρέφει το WorkUnit - Έναρξη, Λήξη και Διάρκεια των εργάσιμων ωρών για το καθορισμένο χρονικό διάστημα. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Επιστρέφει την ποσότητα των εργάσιμων ωρών μεταξύ των καθορισμένων ημερομηνιών. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Επιστρέφει το [`WorkingTimeCollection`](../workingtimecollection/) των ωρών εργασίας για την καθορισμένη ημερομηνία. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Υπολογίζει την έναρξη του επόμενου εργάσιμου χρόνου ξεκινώντας από την καθορισμένη ημερομηνία και ώρα. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Καθορίζει εάν η καθορισμένη ημέρα είναι εργάσιμη ημέρα σύμφωνα με το ημερολόγιο. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Επιστρέφει εάν το ημερολόγιο δεν έχει ορισμένες εργάσιμες ώρες. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


