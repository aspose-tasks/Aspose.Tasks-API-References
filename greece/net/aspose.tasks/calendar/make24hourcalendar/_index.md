---
title: "Calendar.Make24HourCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Μετατρέπει ένα δεδομένο Calendar σε 24ωρο ημερολόγιο. Το 24ωρο ημερολόγιο είναι ένα ημερολόγιο στο οποίο κάθε ημέρα της εβδομάδας εργάζεται με αδιάλειπτες ώρες εργασίας."
type: docs
weight: 10
url: /el/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Κάνει ένα δεδομένο Calendar να είναι ένα 24Ωρο Calendar. Το 24Ωρο Calendar είναι ένα ημερολόγιο στο οποίο κάθε ημέρα της εβδομάδας λειτουργεί με αδιάλειπτες ώρες εργασίας.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερολόγιο | Calendar | Calendar για δημιουργία 24 ωρών ημερολογίου από. |

### Τιμή Επιστροφής

24ωρο Ημερολόγιο.

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα ημερολόγιο 24 ωρών.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Οι 24 ώρες θα εκτυπωθούν
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Δείχνει πώς να μετατρέψετε ένα νέο ημερολόγιο σε ημερολόγιο 24 ωρών.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Οι 24 ώρες θα εκτυπωθούν
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


