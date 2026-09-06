---
title: "Énumération Interval"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Interval enum. Spécifie les intervalles récurrents pour afficher les lignes de progression."
type: docs
weight: 3170
url: /fr/net/aspose.tasks.visualization/interval/
---
## Interval enumeration

Spécifie les intervalles récurrents pour afficher les lignes de progression.

```csharp
public enum Interval
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Daily | `0` | Indique l'intervalle quotidien. |
| Weekly | `1` | Indique l'intervalle hebdomadaire. |
| Monthly | `2` | Indique l'intervalle mensuel. |

## Exemples

Montre comment travailler avec l'intervalle récurrent des lignes de progression.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// lis la ligne de progression
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// redéfinissons l'intervalle récurrent
var newInterval = new RecurringInterval();

// définir une valeur indiquant s'il faut afficher les lignes de progression mensuelles par jour.
interval.MonthlyDay = true;
// définir le numéro du jour des lignes de progression mensuelles.
interval.MonthlyDayDayNumber = 1;
// définir le numéro du mois des lignes de progression mensuelles.
interval.MonthlyDayMonthNumber = 1;
// définir une valeur indiquant s'il faut afficher les lignes de progression par le premier ou le dernier jour prédéfini.
interval.MonthlyFirstLast = true;
// définir le type du premier ou du dernier jour des lignes de progression mensuelles.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// définir le numéro du mois des lignes de progression, qui sont affichées par le premier ou le dernier jour prédéfini.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


