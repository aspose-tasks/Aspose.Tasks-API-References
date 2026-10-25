---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Maakt een gegeven Calendar tot Night Shift Calendar"
type: docs
weight: 20
url: /nl/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Maakt een opgegeven kalender tot nachtploekalender.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| kalender | Calendar | Calendar om Night Shift Calendar te maken. |

### Retourwaarde

Night Shift Calendar.

## Voorbeelden

Toont hoe een night shift calendar te maken.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// toon werktijden
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Toont hoe een calendar om te zetten in een night shift calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// toon werktijden
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


