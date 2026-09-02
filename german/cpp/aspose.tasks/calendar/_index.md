---
title: "Aspose::Tasks::Calendar Klasse"
linktitle: "Kalender"
articleTitle: "Kalender"
second_title: "Aspose.Tasks für C++"
description: "Stellt einen im Projekt verwendeten Kalender dar."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Stellt einen im Projekt verwendeten Kalender dar.

Wie man einen einfachen Kalender von Grund auf erstellt.

```cpp
[C#]
// leeren Kalender erstellen
Calendar calendar = new Calendar("New calendar");
// fügt Standardarbeitstage hinzu (8 Arbeitsstunden von 9:00 bis 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// neuen Arbeitstag erstellen
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Setzt Arbeitszeit. Nur der Zeitanteil von DateTime ist wichtig.
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
// Wochenende hinzufügen
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

Kalender werden verwendet, um standardmäßige Arbeits- und Nichtarbeitszeiten zu definieren. Projekte müssen einen Basis‑Kalender haben. Aufgaben und Ressourcen können eigene Nicht‑Basis‑Kalender besitzen, die auf einem Basis‑Kalender basieren.

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Delete](./delete/) | Entfernt den Kalender aus dem Projekt. |
| [Equals](./equals/) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [get_BaseCalendar](./get_basecalendar/) | Ruft den Basiskalender ab, von dem dieser Kalender abhängt. Nur anwendbar, wenn der Kalender kein Basiskalender ist. |
| [get_Exceptions](./get_exceptions/) | Ruft das CalendarExceptionCollection-Objekt ab. Die Sammlung von Ausnahmen, die dem Kalender zugeordnet ist. |
| [get_Guid](./get_guid/) | Ruft die GUID des Kalenders ab. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Ruft einen Wert ab, der angibt, ob der Kalender ein Basiskalender ist. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Ruft einen Wert ab, der angibt, ob der Kalender ein Baseline‑Kalender ist. |
| [get_Name](./get_name/) | Ruft den Namen des Kalenders ab. |
| [get_Uid](./get_uid/) | Ruft die eindeutige Kennung des Kalenders ab. |
| [get_WeekDays](./get_weekdays/) | Ruft die WeekDaysCollection für diesen Kalender ab. Die Sammlung von Wochentagen, die den Kalender definiert. |
| [get_WorkWeeks](./get_workweeks/) | Ruft das WorkWeekCollections-Objekt ab. Die Sammlung von Arbeitswochen, die dem Kalender zugeordnet ist. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Berechnet das Datum, an dem die angegebene Arbeitszeit gemäß dem Kalender verstrichen ist. |
| [GetHashCode](./gethashcode/) | Gibt einen Hashcode für die Instanz der Klasse zurück. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Ruft die ICalendar-Instanz ab, die verwendet werden kann, um Berechnungen für die Schnittmenge von Arbeitsplänen zweier Kalender durchzuführen. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Berechnet den Beginn des nächsten Arbeitstages für das angegebene Datum. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Berechnet das Ende des vorherigen Arbeitstages vom angegebenen Datum aus. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Berechnet das Enddatum und die Endzeit der Aufgabe aus ihrem Startdatum, den aufgeteilten Teilen und der Arbeitsdauer. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Gibt die Anzahl der Arbeitsstunden am angegebenen Datum zurück. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Gibt die Anzahl der Arbeitsstunden zwischen den angegebenen Daten zurück. |
| [GetWorkingTimes](./getworkingtimes/) | Gibt die WorkingTimeCollection der Arbeitszeiten für das angegebene Datum zurück. |
| [GetWorkStart](./getworkstart/) | Berechnet den Beginn der nächsten Arbeitszeit, beginnend mit dem angegebenen Datum und der Uhrzeit. |
| [IsDayWorking](./isdayworking/) | Bestimmt, ob der angegebene Tag gemäß dem Kalender ein Arbeitstag ist. |
| [IsEmpty](./isempty/) | Gibt zurück, ob der Kalender keine Arbeitszeiten definiert hat. |
| [Make24HourCalendar](./make24hourcalendar/) | Macht einen angegebenen Kalender zu einem 24‑Stunden‑Kalender. Ein 24‑Stunden‑Kalender ist ein Kalender, bei dem jeder Wochentag rund um die Uhr arbeitet. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Macht einen angegebenen Kalender zu einem Nachtschicht‑Kalender. |
| [MakeStandardCalendar](./makestandardcalendar/) | Erstellt den standardmäßigen Standardkalender. |
| [set_BaseCalendar](./set_basecalendar/) | Legt den Basiskalender fest, von dem dieser Kalender abhängt. Nur anwendbar, wenn der Kalender kein Basiskalender ist. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Legt einen Wert fest, der angibt, ob der Kalender ein Baseline‑Kalender ist. |
| [set_Name](./set_name/) | Legt den Namen des Kalenders fest. |
| [set_Uid](./set_uid/) | Legt die eindeutige Kennung des Kalenders fest. |

