---
title: "Aspose.Tasks.Visualization.Gridlines class. Vertegenwoordigt rasterlijnen die verschijnen in een GanttChart‑weergave."
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt het getal op of stelt het in van 0 tot 99 dat het interval tussen rasterlijnen specificeert."
type: docs
weight: 3120
url: /nl/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Stelt rasterlijnen voor die verschijnen in een Gantt‑diagramweergave.

```csharp
public class Gridlines
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Gridlines](gridlines/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Haalt de kleur op of stelt deze in van secundaire rasterlijnen. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Krijgt of stelt de kleur van secundaire rasterlijnen in. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Geeft of stelt het lijnpatroon in voor secundaire rasterlijnen. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Geeft of stelt de kleur in van normale rasterlijnen. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Geeft of stelt het lijnpatroon in voor normale rasterlijnen. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Geeft of stelt het rasterlijntype in. |

## Voorbeelden

Toont hoe te werken met rasterlijnen.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// Stelt de eerste rasterlijn van de weergave in.
var gridlines = view.Gridlines[0];
// Stel het getal van 0 tot 99 in dat het interval tussen rasterlijnen specificeert.
gridlines.Interval = 2;
// Stel de kleur in van secundaire rasterlijnen.
gridlines.IntervalColor = Color.Red;
// Stel het lijnpatroon in voor secundaire rasterlijnen.
gridlines.IntervalPattern = LinePattern.Solid;
// Stel de kleur in van normale rasterlijnen.
gridlines.NormalColor = Color.Blue;
// Stel het lijnpatroon in voor normale rasterlijnen.
gridlines.NormalPattern = LinePattern.CloseDot;
// Stel het rasterlijntype in.
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


