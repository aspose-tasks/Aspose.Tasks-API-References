---
title: "Gridline.Color"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Gridline. Obtiene o establece el Color de una línea de cuadrícula."
type: docs
weight: 20
url: /es/net/aspose.tasks.visualization/gridline/color/
---
## Gridline.Color property

Obtiene o establece el `Color` de una línea de cuadrícula.

```csharp
public Color Color { get; set; }
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

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


