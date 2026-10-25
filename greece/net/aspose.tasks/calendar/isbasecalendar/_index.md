---
title: "Calendar.IsBaseCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι βασικό ημερολόγιο"
type: docs
weight: 70
url: /el/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Λαμβάνει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι βασικό ημερολόγιο.

```csharp
public bool IsBaseCalendar { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα ημερολόγια έργου και τις ιδιότητές τους.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Εμφανίζει εάν υπάρχει βασικό ημερολόγιο.
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Λάβετε τον χρόνο σε ώρες για κάθε εργάσιμη ημέρα.
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


