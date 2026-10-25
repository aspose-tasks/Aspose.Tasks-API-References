---
title: "Κλάση CalendarExceptionCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.CalendarExceptionCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων CalendarException"
type: docs
weight: 260
url: /el/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`CalendarException`](../calendarexception/)

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `CalendarExceptionCollection`. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | Λαμβάνει το γονικό ημερολόγιο για αυτό το αντικείμενο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | Προσθέτει την παρουσία CalendarException σε αυτό το αντικείμενο συλλογής. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | Προσθέτει εύρος εξαιρέσεων στην εσωτερική λίστα. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | Αφαιρεί όλα τα στοιχεία από το `CalendarExceptionCollection`. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | Αφαιρεί την παρουσία [`CalendarException`](../calendarexception/) από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | Μετατρέπει το αντικείμενο CalendarExceptionCollection σε λίστα αντικειμένων [`CalendarException`](../calendarexception/). |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη συλλογή εξαιρέσεων ημερολογίου για να ορίσετε εξαιρέσεις ημερολογίου.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// αφαιρέστε όλες τις εξαιρέσεις
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### Δείτε επίσης

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


