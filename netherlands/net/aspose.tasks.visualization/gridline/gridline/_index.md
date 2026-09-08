---
title: "Gridline.Gridline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Gridline constructor. Initialiseert een nieuw exemplaar van de Gridline-klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

Initialiseert een nieuw exemplaar van de [`Gridline`](../) klasse.

```csharp
public Gridline()
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

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


