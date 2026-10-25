---
title: "RecurringInterval.MonthlyDayDayNumber"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété RecurringInterval. Obtient ou définit le numéro du jour des lignes de progression mensuelles"
type: docs
weight: 60
url: /fr/net/aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/
---
## RecurringInterval.MonthlyDayDayNumber property

Obtient ou définit le numéro du jour des lignes de progression mensuelles.

```csharp
public int MonthlyDayDayNumber { get; set; }
```

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

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


