---
title: "Aspose::Tasks::Calendar klasse"
linktitle: "Kalender"
articleTitle: "Kalender"
second_title: "Aspose.Tasks voor C++"
description: "Stelt een kalender voor die in een project wordt gebruikt."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Stelt een kalender voor die in een project wordt gebruikt.

Hoe een eenvoudige kalender vanaf nul te maken.

```cpp
[C#]
// lege kalender maken
Calendar calendar = new Calendar("New calendar");
// voegt standaard werkdagen toe (8 werkuren van 9:00 tot 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// maak een nieuwe nieuwe werkdag
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

```cpp
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

Kalenders worden gebruikt om standaard werk- en niet-werktijden te definiëren. Projecten moeten één basisagenda hebben. Taken en resources kunnen hun eigen niet-basis kalenders hebben die gebaseerd zijn op een basisagenda.

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Delete](./delete/) | Verwijdert kalender uit project. |
| [Equals](./equals/) | Geeft een waarde terug die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [get_BaseCalendar](./get_basecalendar/) | Haalt de basisagenda op waarop deze agenda is gebaseerd. Alleen van toepassing als de agenda geen basisagenda is. |
| [get_Exceptions](./get_exceptions/) | Haalt het CalendarExceptionCollection-object op. De verzameling uitzonderingen die aan de agenda zijn gekoppeld. |
| [get_Guid](./get_guid/) | Haalt de GUID van de agenda op. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Haalt een waarde op die aangeeft of de agenda een basisagenda is. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Haalt een waarde op die aangeeft of de agenda een baseline-agenda is. |
| [get_Name](./get_name/) | Haalt de naam van de agenda op. |
| [get_Uid](./get_uid/) | Haalt de unieke identifier van de agenda op. |
| [get_WeekDays](./get_weekdays/) | Haalt de WeekDaysCollection voor deze agenda op. De verzameling weekdagen die de agenda definieert. |
| [get_WorkWeeks](./get_workweeks/) | Haalt het WorkWeekCollections-object op. De verzameling werkweken die aan de agenda zijn gekoppeld. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Berekent de datum waarop de opgegeven hoeveelheid werktijd zal verstrijken volgens de kalender. |
| [GetHashCode](./gethashcode/) | Retourneert een hashcode voor de instantie van de klasse. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Haalt de ICalendar-instantie op die kan worden gebruikt om berekeningen uit te voeren op de intersectie van werkschema's van 2 agenda's. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Berekent de start van de volgende werkdag voor de opgegeven datum. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Berekent het einde van de vorige werkdag vanaf de opgegeven datum. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Retourneert de startdatum op basis van de opgegeven einddatum en duur. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Berekent de einddatum en -tijd van de taak op basis van de startdatum, gesplitste delen en de werktijdduur. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Retourneert het aantal werkuren op de opgegeven datum. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Retourneert het aantal werkuren tussen de opgegeven datums. |
| [GetWorkingTimes](./getworkingtimes/) | Retourneert WorkingTimeCollection van werktijden voor de opgegeven datum. |
| [GetWorkStart](./getworkstart/) | Berekent de start van de volgende werktijd beginnend vanaf de opgegeven datum en tijd. |
| [IsDayWorking](./isdayworking/) | Bepaalt of de opgegeven dag een werkdag is volgens de kalender. |
| [IsEmpty](./isempty/) | Geeft terug of de agenda geen werkuren heeft gedefinieerd. |
| [Make24HourCalendar](./make24hourcalendar/) | Maakt een opgegeven agenda tot een 24-uur agenda. Een 24-uur agenda is een agenda waarin elke dag van de week werkt met doorlopende werktijden. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Maakt een opgegeven agenda tot een nachtdienstagenda. |
| [MakeStandardCalendar](./makestandardcalendar/) | Maakt een standaard agenda aan. |
| [set_BaseCalendar](./set_basecalendar/) | Stelt de basisagenda in waarop deze agenda is gebaseerd. Alleen van toepassing als de agenda geen basisagenda is. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Stelt een waarde in die aangeeft of de agenda een baseline-agenda is. |
| [set_Name](./set_name/) | Stelt de naam van de agenda in. |
| [set_Uid](./set_uid/) | Stelt de unieke identifier van de agenda in. |

