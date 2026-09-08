---
title: "Calendar.Make24HourCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Maakt een gegeven kalender tot een 24‑uurkalender. Een 24‑uurkalender is een kalender waarin elke weekdag werkt met de klok rond werktijden"
type: docs
weight: 10
url: /nl/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Maakt een gegeven Kalender tot een 24‑uur Kalender. Een 24‑uur Kalender is een Kalender waarin elke dag van de week werkt met doorlopende werktijden.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| kalender | Calendar | Kalender om een 24-uurskalender van te maken. |

### Retourwaarde

24-uurskalender.

## Voorbeelden

Toont hoe een 24-uurskalender te maken.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 uur wordt afgedrukt
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Toont hoe een nieuwe kalender om te zetten in een 24-uurskalender.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 uur wordt afgedrukt
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


