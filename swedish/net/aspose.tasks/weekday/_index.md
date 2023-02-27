---
title: Class WeekDay
second_title: Aspose.Tasks för .NET API-referens
description: Aspose.Tasks.WeekDay klass. Representerar en veckodag som antingen definierar vanliga veckodagar eller undantagsdagar i en kalender.
type: docs
weight: 3180
url: /sv/net/aspose.tasks/weekday/
---
## WeekDay class

Representerar en veckodag som antingen definierar vanliga veckodagar eller undantagsdagar i en kalender.

```csharp
public class WeekDay
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Initierar en ny instans av`WeekDay` class. |
| [WeekDay](weekday/#constructor_1)(DayType) | Initierar en ny instans av`WeekDay` klass med angiven dagtyp. |
| [WeekDay](weekday/#constructor_2)(DayType, IEnumerable&lt;WorkingTime&gt;) | Initierar en ny instans av`WeekDay` klass med angiven dagtyp och lista över arbetstidsperioder. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Får typen av en dag. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Hämtar eller ställer in ett värde som anger om den angivna datum- eller dagtypen fungerar. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Hämtar eller ställer in början på en undantagstid. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Hämtar eller ställer in slutet på en undantagstid. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Hämtar WorkingTimeCollection för denna WeekDay-instans. Samlingen av arbetstider som definierar den arbetade tiden på veckodagen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Skapar standardarbetsdag. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Returnerar en djup kopia av veckodagen. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Returnerar ett värde som anger om denna instans är lika med ett angivet objekt. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Returnerar ett hashkodvärde för instansen av`WeekDay` class. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Returnerar arbetstiden för en veckodag. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Casts .Net'sDayOfWeek till[`DayType`](./daytype/) . |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Anger standardtidsperioder för den angivna veckodagen. |

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks/)
* hopsättning [Aspose.Tasks](../../)


