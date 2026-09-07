---
title: "Enum TimeUnitType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.TimeUnitType. Specifica il tipo di unità di tempo"
type: docs
weight: 2570
url: /it/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Specifica il tipo di unità di tempo.

```csharp
public enum TimeUnitType : sbyte
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica che il valore Undefined significa che il campo non è stato definito nel file di progetto originale. |
| Minute | `0` | Indica il tipo di unità di tempo Minuto. |
| ElapsedMinute | `1` | Indica il tipo di unità di tempo Minuto trascorso. |
| Hour | `2` | Indica il tipo di unità di tempo Ora. |
| ElapsedHour | `3` | Indica il tipo di unità di tempo Ora trascorsa. |
| Day | `4` | Indica il tipo di unità di tempo Giorno. |
| ElapsedDay | `5` | Indica il tipo di unità di tempo Giorno trascorso. |
| Week | `6` | Indica il tipo di unità di tempo Settimana. |
| ElapsedWeek | `7` | Indica il tipo di unità di tempo Settimana trascorsa. |
| Month | `8` | Indica il tipo di unità di tempo Mese. |
| ElapsedMonth | `9` | Indica il tipo di unità di tempo Mese trascorso. |
| Percent | `10` | Indica il tipo di unità di tempo Percentuale. |
| ElapsedPercent | `11` | Indica il tipo di unità di tempo Percentuale trascorsa. |
| Null | `12` | Indica il tipo di unità di tempo Null. |
| MinuteEstimated | `13` | Indica il tipo di unità di tempo Minuto stimato. |
| ElapsedMinuteEstimated | `14` | Indica il tipo di unità di tempo Minuto stimato trascorso. |
| HourEstimated | `15` | Indica il tipo di unità di tempo Ora stimata. |
| ElapsedHourEstimated | `16` | Indica il tipo di unità di tempo Ora stimata trascorsa. |
| DayEstimated | `17` | Indica il tipo di unità di tempo Giorno stimato. |
| ElapsedDayEstimated | `18` | Indica il tipo di unità di tempo Giorno stimato trascorso. |
| WeekEstimated | `19` | Indica il tipo di unità di tempo Settimana stimata. |
| ElapsedWeekEstimated | `20` | Indica il tipo di unità di tempo Settimana stimata trascorsa. |
| MonthEstimated | `21` | Indica il tipo di unità di tempo Mese stimato. |
| ElapsedMonthEstimated | `22` | Indica il tipo di unità di tempo Mese stimato trascorso. |
| PercentEstimated | `23` | Indica il tipo di unità di tempo Percentuale stimata. |
| ElapsedPercentEstimated | `24` | Indica il tipo di unità di tempo stimata in percentuale trascorsa. |
| Year | `25` | Indica il tipo di unità di tempo Anno. |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come convertire una durata in diversi tipi di unità di tempo.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Ottieni un'attività per calcolare la sua durata in diversi formati
var task = project.RootTask.Children.GetById(1);

// Ottieni la durata in minuti, giorni, ore, settimane e mesi
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


