---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WeekDay methode. Stelt de standaardtijdvakken in voor de opgegeven weekdag"
type: docs
weight: 130
url: /nl/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Stelt standaard tijdsperioden in voor de opgegeven weekdag.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dag | WeekDay | De weekdag waarop de standaardwerkdag moet worden ingesteld. |

## Voorbeelden

Toont hoe een standaardwerktijd voor een dag in te stellen.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// laten we alle werktijden afdrukken
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Zie ook

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


