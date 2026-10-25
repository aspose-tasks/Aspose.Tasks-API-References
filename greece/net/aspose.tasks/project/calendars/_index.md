---
title: "Project.Calendars"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει το αντικείμενο CalendarCollection αυτής της παρουσίας του Project."
type: docs
weight: 130
url: /el/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Λαμβάνει το αντικείμενο [`CalendarCollection`](../../calendarcollection/) αυτής της παρουσίας του Project.

```csharp
public CalendarCollection Calendars { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα ημερολόγια του έργου.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


