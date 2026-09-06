---
title: "GanttChartView.GanttChartView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur GanttChartView. Initialise une nouvelle instance de la classe GanttChartView"
type: docs
weight: 10
url: /fr/net/aspose.tasks/ganttchartview/ganttchartview/
---
## GanttChartView constructor

Initialise une nouvelle instance de la classe [`GanttChartView`](../).

```csharp
public GanttChartView()
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

### Voir aussi

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


