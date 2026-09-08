---
title: "Gridline.Color"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Gridline eigenschap. Haalt de Color van een rasterlijn op of stelt deze in."
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/gridline/color/
---
## Gridline.Color property

Haalt de `Color` van een rasterlijn op of stelt deze in.

```csharp
public Color Color { get; set; }
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


