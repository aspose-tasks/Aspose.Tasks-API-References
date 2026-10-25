---
title: "Enum TimeUnitType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TimeUnitType enum. Specificeert het type van een tijdseenheid"
type: docs
weight: 2570
url: /nl/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Specificeert het type van een tijdseenheid.

```csharp
public enum TimeUnitType : sbyte
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft aan dat een ongedefinieerde waarde betekent dat het veld niet is gedefinieerd in het oorspronkelijke projectbestand. |
| Minute | `0` | Geeft het tijdseenheidtype Minuut aan. |
| ElapsedMinute | `1` | Geeft het tijdseenheidtype Verstreken minuut aan. |
| Hour | `2` | Geeft het tijdseenheidtype Uur aan. |
| ElapsedHour | `3` | Geeft het tijdseenheidtype Verstreken uur aan. |
| Day | `4` | Geeft het tijdseenheidtype Dag aan. |
| ElapsedDay | `5` | Geeft het tijdseenheidtype Verstreken dag aan. |
| Week | `6` | Geeft het tijdseenheidtype Week aan. |
| ElapsedWeek | `7` | Geeft het tijdseenheidtype Verstreken week aan. |
| Month | `8` | Geeft het tijdseenheidtype Maand aan. |
| ElapsedMonth | `9` | Geeft het tijdseenheidtype Verstreken maand aan. |
| Percent | `10` | Geeft het tijdseenheidtype Procent aan. |
| ElapsedPercent | `11` | Geeft het tijdseenheidtype Verstreken procent aan. |
| Null | `12` | Geeft het tijdseenheidtype Null aan. |
| MinuteEstimated | `13` | Geeft het geschatte tijdseenheidtype Minuut aan. |
| ElapsedMinuteEstimated | `14` | Geeft het geschatte tijdseenheidtype Verstreken minuut aan. |
| HourEstimated | `15` | Geeft het geschatte tijdseenheidtype Uur aan. |
| ElapsedHourEstimated | `16` | Geeft het geschatte tijdseenheidtype Verstreken uur aan. |
| DayEstimated | `17` | Geeft het geschatte tijdseenheidtype Dag aan. |
| ElapsedDayEstimated | `18` | Geeft het geschatte tijdseenheidtype Verstreken dag aan. |
| WeekEstimated | `19` | Geeft het geschatte tijdseenheidtype Week aan. |
| ElapsedWeekEstimated | `20` | Geeft het geschatte tijdseenheidtype Verstreken week aan. |
| MonthEstimated | `21` | Geeft het geschatte tijdseenheidtype Maand aan. |
| ElapsedMonthEstimated | `22` | Geeft het geschatte tijdseenheidtype Verstreken maand aan. |
| PercentEstimated | `23` | Geeft het geschatte tijdseenheidtype Procent aan. |
| ElapsedPercentEstimated | `24` | Geeft het type geschatte tijdseenheid voor verstreken percentage aan. |
| Year | `25` | Geeft het type tijdseenheid jaar aan. |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe een duur kan worden geconverteerd naar verschillende tijdseenheidstypen.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Verkrijg een taak om de duur in verschillende formaten te berekenen.
var task = project.RootTask.Children.GetById(1);

// Haal de duur op in Minuten, Dagen, Uren, Weken en Maanden.
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


