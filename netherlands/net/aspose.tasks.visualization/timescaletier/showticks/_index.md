---
title: "TimescaleTier.ShowTicks"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TimescaleTier-eigenschap. Haalt op of stelt een waarde in die aangeeft of tikmarkeringen die tijdsperioden in de tier scheiden, moeten worden weergegeven."
type: docs
weight: 70
url: /nl/net/aspose.tasks.visualization/timescaletier/showticks/
---
## TimescaleTier.ShowTicks property

Haalt op of stelt een waarde in die aangeeft of tikmarkeringen die tijdsperioden in de laag scheiden, moeten worden weergegeven.

```csharp
public bool ShowTicks { get; set; }
```

## Voorbeelden

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

* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


