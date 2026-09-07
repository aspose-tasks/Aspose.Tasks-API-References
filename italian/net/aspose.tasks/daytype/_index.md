---
title: "Enum DayType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.DayType. Specifica il giorno della settimana"
type: docs
weight: 450
url: /it/net/aspose.tasks/daytype/
---
## DayType enumeration

Specifica il giorno della settimana.

```csharp
public enum DayType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Exception | `0` | Indica il tipo di giorno Eccezione. |
| Sunday | `1` | Indica il tipo di giorno Domenica. |
| Monday | `2` | Indica il tipo di giorno Lunedì. |
| Tuesday | `3` | Indica il tipo di giorno Martedì. |
| Wednesday | `4` | Indica il tipo di giorno Mercoledì. |
| Thursday | `5` | Indica il tipo di giorno Giovedì. |
| Friday | `6` | Indica il tipo di giorno Venerdì. |
| Saturday | `7` | Indica il tipo di giorno Sabato. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


