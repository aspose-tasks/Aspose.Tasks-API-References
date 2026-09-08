---
title: "Clase Gridlines"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.Gridlines. Representa las líneas de cuadrícula que aparecen en una vista GanttChart."
type: docs
weight: 3120
url: /es/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Representa líneas de cuadrícula que aparecen en una vista de diagrama de Gantt.

```csharp
public class Gridlines
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Gridlines](gridlines/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Obtiene o establece el número de 0 a 99 que especifica el intervalo entre líneas de cuadrícula. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Obtiene o establece el color de las líneas de cuadrícula secundarias. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Obtiene o establece el patrón de línea para las líneas de cuadrícula secundarias. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Obtiene o establece el color de las líneas de cuadrícula normales. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Obtiene o establece el patrón de línea para las líneas de cuadrícula normales. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


