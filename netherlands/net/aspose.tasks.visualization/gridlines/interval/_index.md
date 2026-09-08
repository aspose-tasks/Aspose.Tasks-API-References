---
title: "Gridlines.Interval"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Gridlines-eigenschap. Haalt het getal van 0 tot 99 op dat het interval tussen rasterlijnen aangeeft of stelt dit in"
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/gridlines/interval/
---
## Gridlines.Interval property

Haalt de kleur op of stelt deze in van secundaire rasterlijnen.

```csharp
public int Interval { get; set; }
```

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

* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


