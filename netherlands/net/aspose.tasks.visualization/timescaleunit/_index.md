---
title: "Enum TimescaleUnit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.TimescaleUnit enum. Specificeert de tijdseenheid voor elke laag van een tijdschaal in een Gantt-diagram of andere tijdsgebaseerde weergave."
type: docs
weight: 3460
url: /nl/net/aspose.tasks.visualization/timescaleunit/
---
## TimescaleUnit enumeration

Specificeert de tijdseenheid voor elke laag van een tijdschaal in een Gantt chart of andere tijdsgebaseerde weergave.

```csharp
public enum TimescaleUnit
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `-1` | Geeft None aan. De laag van de tijdschaal is verborgen. |
| Minutes | `0` | Geeft Minuten tijdschaaleenheid aan. |
| Hours | `1` | Geeft Uren tijdschaaleenheid aan. |
| Days | `2` | Geeft Dagen tijdschaaleenheid aan. |
| Weeks | `3` | Geeft Weken tijdschaaleenheid aan. |
| ThirdsOfMonths | `4` | Geeft Derden van maanden tijdschaaleenheid aan. |
| Months | `5` | Geeft Maanden tijdschaaleenheid aan. |
| Quarters | `6` | Geeft Kwartalen van jaren tijdschaaleenheid aan. |
| HalfYears | `7` | Geeft Halve jaren tijdschaaleenheid aan. |
| Years | `8` | Geeft Jaren tijdschaaleenheid aan. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


