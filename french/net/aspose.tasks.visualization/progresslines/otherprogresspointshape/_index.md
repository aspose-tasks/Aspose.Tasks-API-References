---
title: "ProgressLines.OtherProgressPointShape"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProgressLines. Obtient ou définit la forme du point de progression des autres lignes de progression"
type: docs
weight: 150
url: /fr/net/aspose.tasks.visualization/progresslines/otherprogresspointshape/
---
## ProgressLines.OtherProgressPointShape property

Obtient ou définit la forme du point de progression de l’autre ligne de progression.

```csharp
public GanttBarEndShape OtherProgressPointShape { get; set; }
```

## Exemples

Montre comment travailler avec les lignes de progression.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// définissons la ligne de progression
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// définissez la date à partir de laquelle afficher les lignes de progression. Définissons la date d'état du projet.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// définissez une valeur indiquant s'il faut afficher les lignes de progression depuis le début de la date de début du projet
progressLines.BeginAtProjectStart = true;
// définissez le format de date (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// définissez une valeur indiquant s'il faut afficher la ligne de progression à la date actuelle.
progressLines.DisplayAtCurrentDate = true;
// définissez une valeur indiquant s'il faut afficher la ligne de progression à des intervalles récurrents.
progressLines.DisplayAtRecurringIntervals = true;
// définissez une valeur indiquant s'il faut afficher les lignes de progression aux dates sélectionnées
progressLines.DisplaySelected = true;
// définissez une valeur indiquant s'il faut afficher les lignes de progression pour le plan de référence ou réel.
progressLines.IsBaselinePlan = false;
// définissez la police utilisée pour l'étiquette de la ligne de progression.
progressLines.Font = new FontDescriptor("Arial", 10);
// définissez la couleur de ligne pour la ligne de progression actuelle.
progressLines.LineColor = Color.Aquamarine;
// définissez le motif de ligne de la ligne de progression actuelle.
progressLines.LinePattern = LinePattern.Dashed;
// définissez la couleur de l'autre ligne de progression.
progressLines.OtherLineColor = Color.Azure;
// définissez le motif de ligne pour l'autre ligne de progression.
progressLines.OtherLinePattern = LinePattern.Dotted;
// définissez la couleur de l'autre point de progression.
progressLines.OtherProgressPointColor = Color.Red;
// définissez la forme du point de progression de l'autre ligne de progression.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// définissez la couleur du point de progression.
progressLines.ProgressPointColor = Color.Orange;
// définir la forme du point de progression.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// définir l'intervalle récurrent.
progressLines.RecurringInterval = new RecurringInterval();
// définir l'intervalle récurrent.
progressLines.RecurringInterval.Interval = Interval.Daily;
// définir une valeur indiquant s'il faut afficher la date pour chaque ligne de progression.
progressLines.RecurringInterval.DailyDayNumber = 1;
// vérifions les lignes de progression
progressLines.ShowDate = true;

// Classe TimescaleTier
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* enum [GanttBarEndShape](../../ganttbarendshape/)
* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


