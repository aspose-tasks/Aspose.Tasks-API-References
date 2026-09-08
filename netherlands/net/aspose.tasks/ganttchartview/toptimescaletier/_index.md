---
title: "GanttChartView.TopTimescaleTier"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttChartView eigenschap. Haalt de instellingen van de bovenste tijdschaallaag van de weergave op of stelt deze in. TimescaleTier"
type: docs
weight: 190
url: /nl/net/aspose.tasks/ganttchartview/toptimescaletier/
---
## GanttChartView.TopTimescaleTier property

Haalt of stelt de instellingen van de bovenste tijdschaal van de weergave in. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
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

Toont hoe tijdsschaallaaglabels aangepast kunnen worden.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Taakkoppelingen toevoegen
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// tijdsschaallaag aanpassen

// de bovenste laag afstemmen
// stel de bovenste tijdsschaallaag van de Gantt-diagramweergave in.
view.MiddleTimescaleTier = new TimescaleTier();
// stel tijdsschaaleenheid <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> in voor de tijdsschaallaag.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// stel het tijdseenheid-interval in waarin labels voor de laag worden weergegeven.
view.MiddleTimescaleTier.Count = 1;
// stel datumlabel <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> in voor de tijdsschaallaag.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// stel in hoe labels binnen elke tijdsperiode van de laag worden uitgelijnd (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// stel een waarde in die aangeeft of tickmarks die tijdsperioden in de tier scheiden moeten worden weergegeven.
view.MiddleTimescaleTier.ShowTicks = true;
// stel een waarde in die aangeeft of de tier‑labels gebaseerd moeten worden op het fiscale jaar.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// toegevoegd voor betere visualisatie
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// pas de datums van de middelste tier aan
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Gebruik de optie 'Timescale.DefinedInView' om tijdschalen te renderen met tijdschaalinstellingen die in de weergave zijn gedefinieerd (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Zie ook

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


