---
title: "Gridlines.IntervalColor"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Gridlines. Obtiene o establece el color de las líneas de cuadrícula secundarias"
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/gridlines/intervalcolor/
---
## Gridlines.IntervalColor property

Obtiene o establece el color de las líneas de cuadrícula secundarias.

```csharp
public Color IntervalColor { get; set; }
```

## Ejemplos

Muestra cómo trabajar con líneas de cuadrícula.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// permite ajustar la primera línea de cuadrícula de la vista
var gridlines = view.Gridlines[0];
// establece el número de 0 a 99 que especifica el intervalo entre líneas de cuadrícula.
gridlines.Interval = 2;
// establece el color de las líneas de cuadrícula secundarias.
gridlines.IntervalColor = Color.Red;
// establece el patrón de línea para las líneas de cuadrícula secundarias
gridlines.IntervalPattern = LinePattern.Solid;
// establece el color de las líneas de cuadrícula normales
gridlines.NormalColor = Color.Blue;
// establece el patrón de línea para las líneas de cuadrícula normales
gridlines.NormalPattern = LinePattern.CloseDot;
// establece el tipo de línea de cuadrícula
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


