---
title: "GanttChartView.GanttChartView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttChartView constructor. Initialiseert een nieuw exemplaar van de GanttChartView-klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks/ganttchartview/ganttchartview/
---
## GanttChartView constructor

Initialiseert een nieuw exemplaar van de [`GanttChartView`](../)-klasse.

```csharp
public GanttChartView()
```

## Voorbeelden

Toont hoe tijdschaalniveaus aangepast worden.

```csharp
var project = new Project();

// Initialiseer Gantt Chart-weergave
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// stel tijdschaal‑aantal in
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

// voeg Gantt Chart-weergave toe aan project
project.Views.Add(view);

// voeg wat testgegevens toe aan het project
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Gebruik de optie 'Timescale.DefinedInView' om tijdschalen te renderen met behulp van de tijdschaalinstellingen die we hebben ingesteld (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### Zie ook

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


