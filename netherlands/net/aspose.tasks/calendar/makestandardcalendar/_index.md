---
title: "Calendar.MakeStandardCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Maakt een standaardkalender aan"
type: docs
weight: 30
url: /nl/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Maakt een standaardkalender aan.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| kalender | Calendar | Kalender waaruit een standaardkalender wordt gemaakt. |

### Retourwaarde

Kalender met 5 werkdagen (maandag‑vrijdag) met werktijden 8-12 en 13-17.

## Voorbeelden

Toont hoe een standaardkalender te maken.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// toon werktijden
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Toont hoe een kalender met uitzonderingsdagen te maken.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Werk de kalenderinformatie bij
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

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


