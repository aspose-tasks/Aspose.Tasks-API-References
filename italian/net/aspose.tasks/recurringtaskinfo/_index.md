---
title: "Classe RecurringTaskInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.RecurringTaskInfo. Rappresenta i dettagli di un'attività ricorrente in un progetto"
type: docs
weight: 1720
url: /it/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Rappresenta i dettagli di un'attività ricorrente in un progetto.

```csharp
public class RecurringTaskInfo
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Ottiene o imposta un numero di ripetizioni per il modello di ricorrenza giornaliera. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Ottiene o imposta un valore che indica se utilizzare i giorni lavorativi per il modello di ricorrenza giornaliera. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Ottiene o imposta la durata per una singola occorrenza dell'attività ricorrente. l'istanza della classe [`Duration`](./duration/). |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Ottiene o imposta la data di fine delle occorrenze. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Ottiene o imposta un numero di giorni del modello di ricorrenza mensile. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Ottiene o imposta un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal. Può essere uno dei valori dell'enumerazione DayOfWeek. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Ottiene o imposta un numero ordinal del modello di ricorrenza mensile. Può essere uno dei valori dell'enumerazione [`OrdinalNumber`](../ordinalnumber/). |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Ottiene o imposta un numero di ripetizioni per il modello di ricorrenza mensile quando si utilizza il giorno ordinal. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Ottiene o imposta un numero di ripetizioni per il modello di ricorrenza mensile. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Ottiene o imposta un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza mensile. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Ottiene o imposta un numero di occorrenze dell'attività ricorrente. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Ottiene o imposta un modello di ricorrenza dell'attività ricorrente. Può essere uno dei valori dell'enumerazione [`RecurrencePattern`](./recurrencepattern/). |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Ottiene o imposta la data di inizio delle occorrenze. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Ottiene l'attività padre di questa istanza della classe `RecurringTaskInfo`. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Ottiene o imposta un valore che indica se utilizzare la data di fine o un numero di occorrenze per l'attività ricorrente. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Ottiene o imposta una raccolta di giorni utilizzati nel modello di ricorrenza settimanale. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Ottiene o imposta un numero di ripetizioni per il modello di ricorrenza settimanale. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Ottiene o imposta una data per il modello di ricorrenza annuale. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Ottiene o imposta un giorno della settimana del modello di ricorrenza annuale quando si utilizza il giorno ordinal. Può essere uno dei valori dell'enumerazione DayOfWeek. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Ottiene o imposta un mese del modello di ricorrenza annuale quando si utilizza il giorno ordinal. Può essere uno dei valori dell'enumerazione [`Month`](../month/). |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Ottiene o imposta un numero ordinal del modello di ricorrenza annuale. Può essere uno dei valori dell'enumerazione [`OrdinalNumber`](../ordinalnumber/). |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Ottiene o imposta un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza annuale. |

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


