---
title: "GanttChartView.TopTimescaleTier"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttChartView. Obtient ou définit les paramètres du niveau supérieur de l'échelle de temps de la vue. TimescaleTier"
type: docs
weight: 190
url: /fr/net/aspose.tasks/ganttchartview/toptimescaletier/
---
## GanttChartView.TopTimescaleTier property

Obtient ou définit les paramètres du niveau d'échelle de temps supérieur de la vue. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## Exemples

Montre comment modifier les niveaux d'échelle de temps.

```csharp
var project = new Project();

// Initialiser la vue Gantt Chart
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// définir le nombre d'échelles de temps
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// ajouter la vue Gantt Chart au projet
project.Views.Add(view);

// ajouter des données de test au projet
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Utilisez l'option 'Timescale.DefinedInView' pour rendre les échelles de temps en utilisant les paramètres d'échelle que nous avons définis (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

Ajouter des liens de tâche

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// ajuster les niveaux de l'échelle de temps
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ajuster le niveau supérieur

// définir le niveau supérieur de l'échelle de temps de la vue du diagramme de Gantt.
// définir l'unité d'échelle de temps <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> pour le niveau de l'échelle de temps.
view.MiddleTimescaleTier = new TimescaleTier();
// définir l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// définir le libellé de date <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> pour le niveau de l'échelle de temps.
view.MiddleTimescaleTier.Count = 1;
// définir comment aligner les libellés à l'intérieur de chaque période de temps du niveau (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// définir comment aligner les étiquettes dans chaque période de temps du niveau (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// définir une valeur indiquant s'il faut afficher les marques de repère qui séparent les périodes de temps dans le niveau.
view.MiddleTimescaleTier.ShowTicks = true;
// définir une valeur indiquant s'il faut baser les libellés du niveau sur l'exercice fiscal.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// ajouté pour une meilleure visualisation
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// personnaliser les dates du niveau intermédiaire
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Utilisez l'option 'Timescale.DefinedInView' pour rendre les échelles de temps en utilisant les paramètres d'échelle de temps définis dans la vue (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Voir aussi

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


