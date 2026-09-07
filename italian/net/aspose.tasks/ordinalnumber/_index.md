---
title: "Enum OrdinalNumber"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "**Aspose.Tasks.OrdinalNumber** enum. Rappresenta un numero ordinale nell'istanza della classe RecurringTaskInfo"
type: docs
weight: 1140
url: /it/net/aspose.tasks/ordinalnumber/
---
## OrdinalNumber enumeration

Rappresenta un numero ordinale nell'istanza della classe [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
public enum OrdinalNumber
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| First | `1` | Il primo elemento. |
| Second | `2` | Il secondo elemento. |
| Third | `3` | Il terzo elemento. |
| Fourth | `4` | Il quarto elemento. |
| Last | `5` | L'ultimo elemento. |

## Esempi

Mostra come leggere le informazioni ricorrenti delle attività.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// leggi le informazioni ricorrenti delle attività
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    var info = task.RecurringInfo;
    if (info == null)
    {
        continue;
    }

    Console.WriteLine("Start Date: " + info.StartDate);
    Console.WriteLine("Duration: " + info.Duration);
    Console.WriteLine("End Date: " + info.EndDate);
    Console.WriteLine("Daily Repetitions: " + info.DailyRepetitions);
    Console.WriteLine("Daily Use Workdays: " + info.DailyUseWorkdays);
    Console.WriteLine("Monthly Day: " + info.MonthlyDay);
    Console.WriteLine("Monthly Ordinal Day: " + info.MonthlyOrdinalDay);
    Console.WriteLine("Monthly Ordinal Number: " + info.MonthlyOrdinalNumber);
    Console.WriteLine("Monthly Ordinal Repetitions: " + info.MonthlyOrdinalRepetitions);
    Console.WriteLine("Monthly Repetitions: " + info.MonthlyRepetitions);
    Console.WriteLine("Monthly Use Ordinal Day: " + info.MonthlyUseOrdinalDay);
    Console.WriteLine("Occurrences: " + info.Occurrences);
    Console.WriteLine("Recurrence Pattern: " + info.RecurrencePattern);
    Console.WriteLine("Parent Task: " + info.Task.Get(Tsk.Name));
    Console.WriteLine("Use End Date: " + info.UseEndDate);
    Console.WriteLine("Weekly Days: " + info.WeeklyDays);
    Console.WriteLine("Weekly Repetitions: " + info.WeeklyRepetitions);
    Console.WriteLine("Yearly Date: " + info.YearlyDate);
    Console.WriteLine("Yearly Ordinal Day: " + info.YearlyOrdinalDay);
    Console.WriteLine("Yearly Ordinal Month: " + info.YearlyOrdinalMonth);
    Console.WriteLine("Yearly Ordinal Number: " + info.YearlyOrdinalNumber);
    Console.WriteLine("Yearly Use Ordinal Day: " + info.YearlyUseOrdinalDay);
    Console.WriteLine();
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


