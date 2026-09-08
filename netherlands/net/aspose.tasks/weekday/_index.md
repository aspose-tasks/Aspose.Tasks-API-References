---
title: "Klasse WeekDay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WeekDay klasse. Vertegenwoordigt een weekdag die ofwel reguliere dagen van een week definieert of uitzonderingsdagen in een kalender."
type: docs
weight: 3540
url: /nl/net/aspose.tasks/weekday/
---
## WeekDay class

Stelt een weekdag voor die ofwel reguliere dagen van een week definieert of uitzonderingsdagen in een kalender.

```csharp
public class WeekDay
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Initialiseert een nieuw exemplaar van de `WeekDay` klasse. |
| [WeekDay](weekday/#constructor_1)(DayType) | Initialiseert een nieuw exemplaar van de `WeekDay` klasse met het opgegeven dagtype. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Initialiseert een nieuw exemplaar van de `WeekDay` klasse met het opgegeven dagtype en een lijst van werkperiode‑tijden. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Initialiseert een nieuw exemplaar van de `WeekDay` klasse met het opgegeven dagtype en werkperiode‑tijden. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Haalt het type van een dag op. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of de opgegeven datum of het dagtype een werkdag is. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Haalt het begin van een uitzonderingsperiode op of stelt het in. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Haalt het einde van een uitzonderingsperiode op of stelt het in. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Haalt de WorkingTimeCollection op voor dit WeekDay‑exemplaar. De collectie werkuren die de gewerkte tijd op de weekdag definiëren. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Maakt een standaard werkdag aan. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Retourneert een diepe kopie van de weekdag. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Retourneert een hashcode‑waarde voor het exemplaar van de `WeekDay` klasse. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Retourneert de werktijd voor een weekdag. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Cast .Net's DayOfWeek naar [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Stelt standaard tijdsperioden in voor de opgegeven weekdag. |

## Voorbeelden

Toont hoe een nieuwe kalender te maken door weekdagen te definiëren.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// controleer van‑ en tot‑datums van de uitzonderingsdag
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Stel vrijdag in als korte werkdag

// Stelt werktijd in. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// er is een manier om <see cref=\"DayOfWeek\" /> te converteren naar <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


