---
title: "Calendar.IsBaseCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-eigenschap. Haalt een waarde op die aangeeft of de calendar een basis-calendar is"
type: docs
weight: 70
url: /nl/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Haalt een waarde op die aangeeft of de kalender een basis‑kalender is.

```csharp
public bool IsBaseCalendar { get; }
```

## Voorbeelden

Toont hoe projectkalenders en hun eigenschappen te lezen.

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

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


