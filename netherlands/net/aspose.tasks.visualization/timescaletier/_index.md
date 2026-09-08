---
title: "Klasse TimescaleTier"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.TimescaleTier klasse. Vertegenwoordigt een enkele laag van de tijdsschaal op een Gantt-diagram"
type: docs
weight: 3450
url: /nl/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Stelt een enkel niveau van de tijdschaal op een Gantt‑diagram voor.

```csharp
public sealed class TimescaleTier
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Initialiseert een nieuw exemplaar van de `TimescaleTier` klasse. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Initialiseert een nieuw exemplaar van de `TimescaleTier` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Haalt op of stelt in hoe labels binnen elke tijdsperiode van de laag worden uitgelijnd ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Haalt op of stelt het tijdseenheid-interval in waarin labels voor de laag worden weergegeven. De standaardwaarde is 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Haalt op of stelt een callback-functie in voor het afhandelen van het renderen van datumstippen in deze laag. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Haalt op of stelt datumlabel [`DateLabel`](../datelabel/) in voor de tijdsschaallaag. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Haalt op of stelt een vlag in die bepaalt of datumlabels op elke pagina moeten worden gerenderd wanneer een tijdsperiode zich over meerdere pagina's uitstrekt. Als de waarde 'true' is, worden datumlabels voor de periode op elke pagina weergegeven wanneer de periode zich over meerdere pagina's uitstrekt. Als de waarde 'false' is, wordt het datumlabel slechts één keer weergegeven volgens de waarde van de eigenschap [`Alignment`](./alignment/). |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of tikmarkeringen die tijdsperioden in de laag scheiden, moeten worden weergegeven. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Haalt op of stelt de tijdsschaaleenheid [`TimescaleUnit`](../timescaleunit/) in voor de tijdsschaallaag. De standaardwaarde is [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de laaglabels gebaseerd moeten zijn op het fiscale jaar. |

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


