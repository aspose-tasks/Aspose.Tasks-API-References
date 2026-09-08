---
title: "Gridline.Gridline"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor Gridline. Inicializa una nueva instancia de la clase Gridline."
type: docs
weight: 10
url: /es/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

Inicializa una nueva instancia de la clase [`Gridline`](../).

```csharp
public Gridline()
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


