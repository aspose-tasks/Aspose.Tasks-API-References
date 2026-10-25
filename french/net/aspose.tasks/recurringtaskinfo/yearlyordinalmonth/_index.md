---
title: "RecurringTaskInfo.YearlyOrdinalMonth"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété RecurringTaskInfo. Obtient ou définit un mois du modèle de récurrence annuel lors de l'utilisation du jour ordinal. Peut être l'une des valeurs de l'énumération Month"
type: docs
weight: 200
url: /fr/net/aspose.tasks/recurringtaskinfo/yearlyordinalmonth/
---
## RecurringTaskInfo.YearlyOrdinalMonth property

Obtient ou définit un mois du modèle de récurrence annuel lors de l'utilisation du jour ordinal. Peut être l'une des valeurs de l'énumération [`Month`](../../month/)

```csharp
public Month YearlyOrdinalMonth { get; set; }
```

## Exemples

Montre comment lire les informations récurrentes des tâches.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// lire les informations récurrentes des tâches
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

### Voir aussi

* enum [Month](../../month/)
* class [RecurringTaskInfo](../)
* namespace [Aspose.Tasks](../../recurringtaskinfo/)
* assembly [Aspose.Tasks](../../../)


