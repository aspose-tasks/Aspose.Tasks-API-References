---
title: "Enum Month"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Month enum. Specifica il mese"
type: docs
weight: 1040
url: /it/net/aspose.tasks/month/
---
## Month enumeration

Specifica il mese.

```csharp
public enum Month
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica che il valore non era definito nel file di progetto originale. |
| January | `0` | Indica il mese di gennaio. |
| February | `1` | Indica il mese di febbraio. |
| March | `2` | Indica il mese di marzo. |
| April | `3` | Indica il mese di aprile. |
| May | `4` | Indica il mese di maggio. |
| June | `5` | Indica il mese di giugno. |
| July | `6` | Indica il mese di luglio. |
| August | `7` | Indica il mese di agosto. |
| September | `8` | Indica il mese di settembre. |
| October | `9` | Indica il mese di ottobre. |
| November | `10` | Indica il mese di novembre. |
| December | `11` | Indica il mese di dicembre. |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come lavorare con le ripetizioni giornaliere annuali durante la creazione di nuove attività ricorrenti.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


