---
title: "Gridline.Pattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Gridline eigenschap. Haalt het LinePattern van een rasterlijn op of stelt dit in."
type: docs
weight: 40
url: /nl/net/aspose.tasks.visualization/gridline/pattern/
---
## Gridline.Pattern property

Haalt het [`LinePattern`](../../linepattern/) van een rasterlijn op of stelt dit in.

```csharp
public LinePattern Pattern { get; set; }
```

## Voorbeelden

Toont hoe te werken met rasterlijnen bij het opslaan in visuele formaten.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // stel het type van de rasterlijn in (<see cref="P:Aspose.Tasks.Visualization.Gridline.GridlineType" />).
    GridlineType = GridlineType.GanttRow, 
    // stel de <see cref="T:Aspose.Tasks.Visualization.LinePattern" /> van een rasterlijn in
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Zie ook

* enum [LinePattern](../../linepattern/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


