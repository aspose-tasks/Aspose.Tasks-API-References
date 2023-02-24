---
title: Class Calendar
second_title: Aspose.Tasks för .NET API-referens
description: Aspose.Tasks.Calendar klass. Representerar en kalender som används i ett projekt.
type: docs
weight: 230
url: /sv/net/aspose.tasks/calendar/
---
## Calendar class

Representerar en kalender som används i ett projekt.

```csharp
public class Calendar
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Hämtar eller ställer in baskalendern som denna kalender beror på. Endast tillämpligt om kalendern inte är en baskalender. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Hämtar CalendarExceptionCollection-objekt. Samlingen av undantag som är associerad med kalendern. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Får ett värde som indikerar om kalendern är en baskalender. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Hämtar eller ställer in ett värde som anger om kalendern är en baslinjekalender. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Hämtar eller ställer in namnet på kalendern. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Hämtar eller ställer in den unika identifieraren för kalendern. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Får WeekDaysCollection för denna kalender. Samlingen av veckodagar som definierar kalendern. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Hämtar WorkWeekCollections-objekt. Samlingen av arbetsveckor som är kopplad till kalendern. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Gör en given kalender till en 24-timmarskalender. 24-timmarskalender är en kalender där varje veckodag arbetar med dygnet-runt-arbetstid. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Gör en given kalender som Night Shift Calendar. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Skapar standard standardkalender. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Tar bort kalender från projektet. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Returnerar ett värde som anger om denna instans är lika med ett angivet objekt. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Beräknar datumet då den angivna arbetstiden kommer att passera enligt kalendern. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Beräknar datumet då den angivna arbetstiden kommer att passera enligt kalendern. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Returnerar en hashkod för instansen av klassen. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Beräknar nästa arbetsdag från och med datumet. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Beräknar föregående arbetsdatum slut från det angivna datumet. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Returnerar startdatum baserat på specificerat slutdatum och varaktighet. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Returnerar startdatum baserat på specificerat slutdatum och varaktighet. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Beräknar uppgiftens slutdatum och tid från dess startdatum, delade delar och varaktigheten. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Returnerar antalet arbetstimmar vid datumet. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Returarbetstid för de angivna datumen. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Returnerar[`WorkingTimeCollection`](../workingtimecollection/) av arbetstider för det angivna datumet. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Bestämmer om dagen är arbetsdag. |

### Anmärkningar

Kalendrar används för att definiera vanliga arbetstider och icke-arbetande tider. Projekt måste ha en baskalender. Uppgifter och resurser kan ha sina egna icke-baskalendrar som är baserade på en baskalender.

### Exempel

Hur man skapar en enkel kalender från grunden.

```csharp
[C#]
// skapa en tom kalender
Calendar calendar = new Calendar("New calendar");
// lägger till standardarbetsdagar (8 arbetstimmar från 9:00 till 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// skapa ny ny arbetsdag
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Ställer in arbetstid. Endast tidsdelen av DateTime är viktig
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
// lägger helg
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' skapa en tom kalender
Dim calendar As Calendar =  New Calendar("New calendar")
' lägger till standardarbetsdagar (8 arbetstimmar från 9:00 till 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' skapa ny ny arbetsdag
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Ställer in arbetstid. Endast tidsdelen av DateTime är viktig
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
' lägger helg
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks/)
* hopsättning [Aspose.Tasks](../../)


