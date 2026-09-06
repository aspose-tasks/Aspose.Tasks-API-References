---
title: "Classe ProgressLines"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.ProgressLines. Représente les lignes de progression dans une vue de diagramme de Gantt"
type: docs
weight: 3290
url: /fr/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Représente les lignes de progression dans une vue du diagramme de Gantt.

```csharp
public class ProgressLines
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ProgressLines](progresslines/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | Obtient ou définit la date à partir de laquelle afficher les lignes de progression. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher les lignes de progression depuis le début de la date de début du projet. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Obtient ou définit le format de date ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher la ligne de progression à la date actuelle. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher la ligne de progression à des intervalles récurrents. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher les lignes de progression aux dates sélectionnées. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | Obtient ou définit la police utilisée pour l’étiquette de la ligne de progression. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher les lignes de progression pour le plan de référence ou réel. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Obtient ou définit la couleur de la ligne pour la ligne de progression actuelle. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Obtient ou définit le motif de ligne de la ligne de progression actuelle. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Obtient ou définit la couleur de l’autre ligne de progression. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Obtient ou définit le motif de ligne pour l’autre ligne de progression. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Obtient ou définit la couleur de l’autre point de progression. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Obtient ou définit la forme du point de progression de l’autre ligne de progression. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | Obtient ou définit la couleur du point de progression. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | Obtient ou définit la forme du point de progression. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Obtient ou définit l’intervalle récurrent. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | Obtient la liste des dates sélectionnées pour afficher les lignes de progression. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher la date pour chaque ligne de progression. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


