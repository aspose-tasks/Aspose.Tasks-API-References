---
title: "Classe RecurringInterval"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.RecurringInterval. Représente les intervalles récurrents utilisés dans les lignes de progression d'une vue de diagramme de Gantt"
type: docs
weight: 3310
url: /fr/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Représente les intervalles récurrents utilisés dans les lignes de progression d'une vue du diagramme de Gantt.

```csharp
public class RecurringInterval
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Obtient ou définit le numéro du jour quotidien. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Obtient ou définit une valeur indiquant si un jour est ouvrable pour les lignes de progression quotidiennes. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Obtient ou définit l'intervalle récurrent. Peut être n'importe quelle valeur du type [`Interval`](./interval/). |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher les lignes de progression mensuelles par jour. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Obtient ou définit le numéro du jour des lignes de progression mensuelles. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Obtient ou définit le numéro du mois des lignes de progression mensuelles. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher les lignes de progression par le premier ou le dernier jour prédéfini. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Obtient ou définit le type du premier ou du dernier jour des lignes de progression mensuelles. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Obtient ou définit le numéro du mois des lignes de progression, qui sont affichées par le premier ou le dernier jour prédéfini. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Obtient une liste de jours pour les lignes de progression hebdomadaires. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Obtient ou définit le numéro de la semaine pour les lignes de progression hebdomadaires. |

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


