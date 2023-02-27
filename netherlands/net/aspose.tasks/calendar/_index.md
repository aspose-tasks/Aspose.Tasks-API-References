---
title: Calendar
second_title: Aspose.Tasks voor .NET API-referentie
description: Vertegenwoordigt een kalender die in een project wordt gebruikt.
type: docs
weight: 230
url: /nl/net/aspose.tasks/calendar/
---
## Calendar class

Vertegenwoordigt een kalender die in een project wordt gebruikt.

```csharp
public class Calendar
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Haalt of stelt de basiskalender in waarvan deze kalender afhankelijk is. Alleen van toepassing als de kalender geen basiskalender is. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Haalt het CalendarExceptionCollection-object op. De verzameling uitzonderingen die is gekoppeld aan de kalender. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Krijgt een waarde die aangeeft of de kalender een basiskalender is. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de kalender een basiskalender is. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Haalt de naam van de agenda op of stelt deze in. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Haalt de unieke identificatie van de agenda op of stelt deze in. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Haalt WeekDaysCollection op voor deze agenda. De verzameling weekdagen die de agenda definieert. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Haalt WorkWeekCollections-object op. De verzameling werkweken die aan de kalender is gekoppeld. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Maakt van een bepaalde kalender een 24-uurs kalender. 24-uurs kalender is een kalender waarin elke dag van de week werkt met 24-uurs werkuren. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Maakt een gegeven kalender als Night Shift Calendar. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Creëert standaard standaard kalender. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Verwijdert agenda uit project. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Berekent de datum waarop de opgegeven hoeveelheid werktijd zal verstrijken volgens de kalender. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Berekent de datum waarop de opgegeven hoeveelheid werktijd zal verstrijken volgens de kalender. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Retourneert een hash-code voor de instantie van de klasse. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Berekent de start van de volgende werkdag vanaf de datum. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Berekent het einde van de vorige werkdatum vanaf de opgegeven datum. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Retourneert StartDate op basis van gespecificeerde FinishDate en Duration. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Retourneert StartDate op basis van gespecificeerde FinishDate en Duration. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Berekent de einddatum en -tijd van de taak vanaf de startdatum, gesplitste delen en de duur. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Retourneert het aantal werkuren op de datum. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Retourneer werkuren voor de opgegeven datums. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Retourneert[`WorkingTimeCollection`](../workingtimecollection/) van werktijden voor de opgegeven datum. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Bepaalt of de dag een werkdag is. |

### Opmerkingen

Kalenders worden gebruikt om standaard werk- en rusttijden te definiëren. Projecten moeten één basiskalender hebben. Taken en resources kunnen hun eigen niet-basiskalenders hebben die zijn gebaseerd op een basiskalender.

### Voorbeelden

Hoe maak je een eenvoudige kalender vanuit het niets.

```csharp
[C#]
// maak een lege kalender
Calendar calendar = new Calendar("New calendar");
// voegt standaard werkdagen toe (8 werkuren van 9:00 tot 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// creëer een nieuwe nieuwe werkdag
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Stelt de werktijd in. Alleen het tijdgedeelte van DateTime is belangrijk
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
' lege agenda maken
Dim calendar As Calendar =  New Calendar("New calendar")
' voegt standaard werkdagen toe (8 werkuren van 9:00 tot 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' maak een nieuwe nieuwe werkdag
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Stelt de werktijd in. Alleen het tijdgedeelte van DateTime is belangrijk
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
' weekend toegevoegd
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Zie ook

* naamruimte [Aspose.Tasks](../../aspose.tasks/)
* montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
