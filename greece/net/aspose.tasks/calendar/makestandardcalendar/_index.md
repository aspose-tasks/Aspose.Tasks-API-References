---
title: "Calendar.MakeStandardCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Δημιουργεί προεπιλεγμένο τυπικό ημερολόγιο"
type: docs
weight: 30
url: /el/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Δημιουργεί προεπιλεγμένο τυπικό ημερολόγιο.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερολόγιο | Calendar | Ημερολόγιο από το οποίο θα δημιουργηθεί τυπικό ημερολόγιο. |

### Τιμή Επιστροφής

Ημερολόγιο με 5 εργάσιμες ημέρες (Δευτέρα-Παρασκευή) με ώρες εργασίας 8-12 και 13-17.

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα τυπικό ημερολόγιο.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// εμφάνιση ωρών εργασίας
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Δείχνει πώς να δημιουργήσετε ένα ημερολόγιο με ημέρες εξαιρέσεων.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Ενημερώστε τις πληροφορίες του ημερολογίου
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


