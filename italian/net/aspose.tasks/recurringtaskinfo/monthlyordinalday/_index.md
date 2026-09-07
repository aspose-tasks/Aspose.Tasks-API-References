---
title: "RecurringTaskInfo.MonthlyOrdinalDay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà RecurringTaskInfo. Ottiene o imposta un giorno del modello di ricorrenza mensile quando si usa il giorno ordinal. Può essere uno dei valori dell'enumerazione DayOfWeek"
type: docs
weight: 60
url: /it/net/aspose.tasks/recurringtaskinfo/monthlyordinalday/
---
## RecurringTaskInfo.MonthlyOrdinalDay property

Ottiene o imposta un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal. Può essere uno dei valori dell'enumerazione DayOfWeek.

```csharp
public DayOfWeek MonthlyOrdinalDay { get; set; }
```

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

* class [RecurringTaskInfo](../)
* namespace [Aspose.Tasks](../../recurringtaskinfo/)
* assembly [Aspose.Tasks](../../../)


