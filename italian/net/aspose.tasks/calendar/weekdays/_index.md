---
title: "Calendar.WeekDays"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Ottiene WeekDaysCollection per questo calendario. La raccolta di giorni della settimana che definisce il calendario"
type: docs
weight: 120
url: /it/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Ottiene la WeekDaysCollection per questo calendario. La raccolta dei giorni della settimana che definisce il calendario.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Esempi

Mostra come definire un nuovo calendario, aggiungere i giorni della settimana e definire gli orari di lavoro per i giorni.

```csharp
var project = new Project();

// Definisci un calendario
var calendar = project.Calendars.Add("Calendar1");

// Aggiungi giorni lavorativi da lunedì a giovedì con gli orari predefiniti
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Imposta il venerdì come giorno lavorativo breve
var weekDay = new WeekDay(DayType.Friday);

// Imposta l'orario di lavoro. È importante solo la parte ora di DateTime
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// lavorare con il progetto...
```

### Vedi anche

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


