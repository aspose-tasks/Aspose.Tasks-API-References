---
title: "Project.Calendars"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-eigenschap. Haalt het CalendarCollection-object op van deze Project‑instantie"
type: docs
weight: 130
url: /nl/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Haalt het [`CalendarCollection`](../../calendarcollection/) object op van deze Project‑instantie.

```csharp
public CalendarCollection Calendars { get; }
```

## Voorbeelden

Toont hoe projectkalenders te lezen.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Toon of er een basisagenda is
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Haal de tijd in uren op voor elke werkdag
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### Zie ook

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


