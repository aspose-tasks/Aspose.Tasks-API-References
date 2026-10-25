---
title: "GanttChartView.Gridlines"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GanttChartView. Obtiene o establece una lista de Gridlines de la vista de diagrama de Gantt"
type: docs
weight: 80
url: /es/net/aspose.tasks/ganttchartview/gridlines/
---
## GanttChartView.Gridlines property

Obtiene o establece una lista de `Gridlines` de la vista de diagrama de Gantt.

```csharp
public List<Gridlines> Gridlines { get; set; }
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

* class [Gridlines](../../../aspose.tasks.visualization/gridlines/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


