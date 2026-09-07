---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Δημιουργεί ένα δεδομένο Calendar ως Night Shift Calendar"
type: docs
weight: 20
url: /el/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Μετατρέπει ένα δεδομένο Ημερολόγιο σε Ημερολόγιο Νυχτερινής Βάρδιας.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερολόγιο | Calendar | Calendar για τη δημιουργία Night Shift Calendar. |

### Τιμή Επιστροφής

Night Shift Calendar.

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα night shift calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// εμφάνιση ωρών εργασίας
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Δείχνει πώς να μετατρέψετε ένα ημερολόγιο σε night shift calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// εμφάνιση ωρών εργασίας
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


