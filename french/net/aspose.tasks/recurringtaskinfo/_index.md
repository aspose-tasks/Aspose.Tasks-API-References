---
title: "Classe RecurringTaskInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.RecurringTaskInfo. Représente les détails d'une tâche récurrente dans un projet"
type: docs
weight: 1720
url: /fr/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Représente les détails d'une tâche récurrente dans un projet.

```csharp
public class RecurringTaskInfo
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Obtient ou définit un nombre de répétitions pour le modèle de récurrence quotidien. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut utiliser les jours ouvrés pour le modèle de récurrence quotidien. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Obtient ou définit la durée d'une occurrence de la tâche récurrente. l'instance de la classe [`Duration`](./duration/). |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Obtient ou définit la date de fin des occurrences. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Obtient ou définit un nombre de jours du modèle de récurrence mensuel. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Obtient ou définit un jour du modèle de récurrence mensuel lorsqu'on utilise le jour ordinal. Peut être l'une des valeurs de l'énumération DayOfWeek. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Obtient ou définit un nombre ordinal du modèle de récurrence mensuel. Peut être l'une des valeurs de l'énumération [`OrdinalNumber`](../ordinalnumber/). |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Obtient ou définit un nombre de répétitions pour le modèle de récurrence mensuel lorsqu'on utilise le jour ordinal. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Obtient ou définit un nombre de répétitions pour le modèle de récurrence mensuel. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence mensuel. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Obtient ou définit un nombre d'occurrences de la tâche récurrente. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Obtient ou définit un modèle de récurrence de la tâche récurrente. Peut être l'une des valeurs de l'énumération [`RecurrencePattern`](./recurrencepattern/). |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Obtient ou définit la date de début des occurrences. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Obtient la tâche parente de cette instance de la classe `RecurringTaskInfo`. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut utiliser la date de fin ou un nombre d'occurrences pour la tâche récurrente. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Obtient ou définit une collection de jours utilisés dans le modèle de récurrence hebdomadaire. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Obtient ou définit un nombre de répétitions pour le modèle de récurrence hebdomadaire. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Obtient ou définit une date pour le modèle de récurrence annuel. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Obtient ou définit un jour de la semaine du modèle de récurrence annuel lorsqu'on utilise le jour ordinal. Peut être l'une des valeurs de l'énumération DayOfWeek. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Obtient ou définit un mois du modèle de récurrence annuel lorsqu'on utilise le jour ordinal. Peut être l'une des valeurs de l'énumération [`Month`](../month/). |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Obtient ou définit un numéro ordinal du modèle de récurrence annuel. Peut être l'une des valeurs de l'énumération [`OrdinalNumber`](../ordinalnumber/). |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence annuel. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


