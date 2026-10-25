---
title: "Gridline.GridlineType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Gridline. Obtiene o establece el tipo de línea de cuadrícula GridlineType."
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/gridline/gridlinetype/
---
## Gridline.GridlineType property

Obtiene o establece el tipo de línea de cuadrícula (`GridlineType`).

```csharp
public GridlineType GridlineType { get; set; }
```

## Ejemplos

Muestra cómo trabajar con líneas de cuadrícula al guardar en formatos visuales.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // establece el tipo de línea de cuadrícula (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // establece el <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> de una línea de cuadrícula
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Ver también

* enum [GridlineType](../../gridlinetype/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


