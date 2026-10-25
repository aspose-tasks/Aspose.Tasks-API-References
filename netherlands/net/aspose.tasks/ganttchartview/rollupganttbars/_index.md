---
title: "GanttChartView.RollUpGanttBars"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttChartView-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of balken op het Gantt-diagram moeten worden samengevoegd"
type: docs
weight: 130
url: /nl/net/aspose.tasks/ganttchartview/rollupganttbars/
---
## GanttChartView.RollUpGanttBars property

Haalt op of stelt een waarde in die aangeeft of balken op de Gantt Chart moeten worden samengevoegd.

```csharp
public bool RollUpGanttBars { get; set; }
```

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

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


