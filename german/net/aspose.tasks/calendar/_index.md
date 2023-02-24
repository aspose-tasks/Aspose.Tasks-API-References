---
title: Class Calendar
second_title: Aspose.Tasks für .NET-API-Referenz
description: Aspose.Tasks.Calendar klas. Stellt einen Kalender dar der in einem Projekt verwendet wird.
type: docs
weight: 230
url: /de/net/aspose.tasks/calendar/
---
## Calendar class

Stellt einen Kalender dar, der in einem Projekt verwendet wird.

```csharp
public class Calendar
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Ruft den Basiskalender ab, von dem dieser Kalender abhängt, oder legt ihn fest. Gilt nur, wenn der Kalender kein Basiskalender ist. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Ruft das CalendarExceptionCollection-Objekt ab. Die Sammlung von Ausnahmen, die dem Kalender zugeordnet ist. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Ruft einen Wert ab, der angibt, ob der Kalender ein Basiskalender ist. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Kalender ein Basiskalender ist. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Ruft den Namen des Kalenders ab oder legt ihn fest. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Ruft die eindeutige Kennung des Kalenders ab oder legt sie fest. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Ruft die WeekDaysCollection für diesen Kalender ab. Die Sammlung von Wochentagen, die den Kalender definiert. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Ruft das WorkWeekCollections-Objekt ab. Die Sammlung von Arbeitswochen, die dem Kalender zugeordnet ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Macht einen bestimmten Kalender zu einem 24-Stunden-Kalender. 24-Stunden-Kalender ist ein Kalender, in dem jeder Wochentag mit Arbeitszeiten rund um die Uhr arbeitet. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Macht einen gegebenen Kalender als Nachtschichtkalender. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Erstellt Standard-Standardkalender. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Entfernt den Kalender aus dem Projekt. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Gibt einen Wert zurück, der angibt, ob diese Instanz gleich einem angegebenen Objekt ist. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Berechnet das Datum, an dem die angegebene Arbeitszeit laut Kalender vergehen wird. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Berechnet das Datum, an dem die angegebene Arbeitszeit laut Kalender vergehen wird. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Gibt einen Hashcode für die Instanz der Klasse zurück. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Berechnet den Beginn des nächsten Arbeitstages ab dem Datum. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Berechnet das Ende des vorherigen Arbeitsdatums aus dem angegebenen Datum. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der angegebenen Dauer zurück. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der angegebenen Dauer zurück. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Berechnet das Enddatum und die Endzeit der Aufgabe aus dem Startdatum, aufgeteilten Teilen und der Dauer. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Gibt die Anzahl der Arbeitsstunden zum Datum zurück. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Arbeitsstunden für die angegebenen Daten zurückgeben. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | gibt zurück[`WorkingTimeCollection`](../workingtimecollection/) der Arbeitszeiten für das angegebene Datum. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Bestimmt, ob der Tag ein Arbeitstag ist. |

### Bemerkungen

Kalender werden verwendet, um Standardarbeitszeiten und arbeitsfreie Zeiten zu definieren. Projekte müssen einen Basiskalender haben. Aufgaben und Ressourcen können ihre eigenen Nicht-Basiskalender haben, die auf einem Basiskalender basieren.

### Beispiele

So erstellen Sie einen einfachen Kalender von Grund auf neu.

```csharp
[C#]
// leeren Kalender erstellen
Calendar calendar = new Calendar("New calendar");
// fügt Standardarbeitstage hinzu (8 Arbeitsstunden von 9:00 bis 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// Neuen neuen Arbeitstag erstellen
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Legt die Arbeitszeit fest. Nur der Zeitteil von DateTime ist wichtig
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
// fügt Wochenende hinzu
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' leeren Kalender erstellen
Dim calendar As Calendar =  New Calendar("New calendar")
' fügt Standardarbeitstage hinzu (8 Arbeitsstunden von 9:00 bis 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' Erstellen Sie einen neuen neuen Arbeitstag
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Legt die Arbeitszeit fest. Nur der Zeitteil von DateTime ist wichtig
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
' fügt Wochenende hinzu
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Siehe auch

* namensraum [Aspose.Tasks](../../aspose.tasks/)
* Montage [Aspose.Tasks](../../)


