---
title: "Gridline.GridlineType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Gridline eigenschap. Haalt het type van rasterlijn GridlineType op of stelt dit in."
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/gridline/gridlinetype/
---
## Gridline.GridlineType property

Haalt het type van rasterlijn (`GridlineType`) op of stelt dit in.

```csharp
public GridlineType GridlineType { get; set; }
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

* enum [GridlineType](../../gridlinetype/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


