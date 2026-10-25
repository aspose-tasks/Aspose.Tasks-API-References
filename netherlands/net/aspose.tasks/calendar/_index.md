---
title: "Class Calendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Calendar class. Vertegenwoordigt een kalender die in een project wordt gebruikt."
type: docs
weight: 230
url: /nl/net/aspose.tasks/calendar/
---
## Calendar class

Stelt een kalender voor die in een project wordt gebruikt.

```csharp
public class Calendar : ICalendar
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Haalt op of stelt de basis‑kalender in waarop deze kalender afhankelijk is. Alleen van toepassing als de kalender geen basis‑kalender is. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Haalt CalendarExceptionCollection‑object op. De verzameling uitzonderingen die aan de kalender zijn gekoppeld. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Haalt de Guid van de kalender op. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Haalt een waarde op die aangeeft of de kalender een basis‑kalender is. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de kalender een baseline‑kalender is. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Haalt op of stelt de naam van de kalender in. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Haalt een object op dat Primavera‑specifieke eigenschappen bevat voor een kalender die uit Primavera‑formaten is gelezen. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Haalt op of stelt de unieke identifier van de kalender in. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Haalt WeekDaysCollection op voor deze kalender. De verzameling weekdagen die de kalender definieert. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Haalt WorkWeekCollections‑object op. De verzameling werkweken die aan de kalender zijn gekoppeld. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Maakt een gegeven Kalender tot een 24‑uur Kalender. Een 24‑uur Kalender is een Kalender waarin elke dag van de week werkt met doorlopende werktijden. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Maakt een opgegeven kalender tot nachtploekalender. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Maakt een standaardkalender aan. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Verwijdert kalender uit project. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Retourneert een hashcode voor de instantie van de klasse. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Berekent het begin van de volgende werkdag voor de opgegeven datum. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Berekent het einde van de vorige werkdag vanaf de opgegeven datum. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Retourneert de startdatum op basis van de opgegeven einddatum en duur. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Retourneert de startdatum op basis van de opgegeven einddatum en duur. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Berekent de einddatum en -tijd van de taak op basis van de startdatum, gesplitste delen en de werktijdduur. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Retourneert het aantal werkuren op de opgegeven datum. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Retourneer WorkUnit - Start, Eind en Duur van werktijden voor het opgegeven datum‑tijdinterval. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Retourneert het aantal werkuren tussen de opgegeven datums. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Retourneert [`WorkingTimeCollection`](../workingtimecollection/) van werktijden voor de opgegeven datum. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Berekent het begin van de volgende werktijd vanaf de opgegeven datum en tijd. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Bepaalt of de opgegeven dag een werkdag is volgens de kalender. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Retourneert of de kalender geen werkuren heeft gedefinieerd. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | Haalt [`ICalendar`](../icalendar/) instantie op die kan worden gebruikt om berekeningen uit te voeren op de intersectie van werkschema's van 2 kalenders. |

## Opmerkingen

Kalenders worden gebruikt om standaard werk- en niet‑werktijden te definiëren. Projecten moeten één basis‑kalender hebben. Taken en resources kunnen hun eigen niet‑basis kalenders hebben die zijn gebaseerd op een basis‑kalender.

## Voorbeelden

Hoe maak je een eenvoudige kalender vanaf nul.

```csharp
[C#]
// maak lege kalender
Calendar calendar = new Calendar("New calendar");
// voegt standaard werkdagen toe (8 werkuren van 9:00 tot 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// maak een nieuwe werkdag
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Stelt werktijd in. Alleen het tijdgedeelte van DateTime is belangrijk.
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// voegt weekend toe
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

Toont hoe je een nieuwe kalender definieert, weekdagen toevoegt en werktijden voor dagen definieert.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Stel vrijdag in als korte werkdag
var weekDay = new WeekDay(DayType.Friday);

// Stelt werktijd in. Alleen het tijdgedeelte van DateTime is belangrijk.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// werken met het project...
```

### Zie ook

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


