---
title: "Enum GanttBarSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GanttBarSize enum. Specificeert de hoogte van een balk in punten."
type: docs
weight: 700
url: /nl/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Specificeert de hoogte van een balk in punten.

```csharp
public enum GanttBarSize
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| BarSize6 | `0` | Balkgrootte 6 punten. |
| BarSize8 | `1` | Balkgrootte 8 punten. |
| BarSize10 | `2` | Balkgrootte 10 punten. |
| BarSize12 | `3` | Balkgrootte 12 punten. |
| BarSize14 | `4` | Balkgrootte 14 punten. |
| BarSize18 | `5` | Balkgrootte 18 punten. |
| BarSize24 | `6` | Balkgrootte 24 punten. |

## Voorbeelden

Toont hoe enkele nuttige eigenschappen van de Gantt-diagramweergave in te stellen.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// stel een waarde in die aangeeft of de balken naar de dichtstbijzijnde dag afronden
view.BarRounding = false;
// stel de hoogte, in punten, van de Gantt-balken in het Gantt-diagram in
view.BarSize = GanttBarSize.BarSize24;
// stel een waarde in die aangeeft of roll-up balken verborgen worden bij het uitvouwen van een samenvattende taak
view.HideRollupBarsWhenSummaryExpanded = true;
// stel de kleur van niet-werkelijke tijd in
view.NonWorkingTimeColor = Color.Azure;
// stel een waarde in die aangeeft of balken op het Gantt-diagram moeten worden opgerold
view.RollUpGanttBars = true;
// stel een waarde in die aangeeft of taakonderbrekingen op het Gantt-diagram moeten worden weergegeven
view.ShowBarSplits = true;
// stel een waarde in die aangeeft of tekeningen op het Gantt-diagram moeten worden weergegeven
view.ShowDrawings = true;
// stel een percentage in om de afstand tussen eenheden op de tijdschaallaag te verkleinen of te vergroten
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


