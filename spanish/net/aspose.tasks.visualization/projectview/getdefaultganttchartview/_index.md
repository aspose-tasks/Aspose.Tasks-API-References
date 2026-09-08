---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectView. Incluye indicadores de id, nombre, duración, inicio y fin de columnas de tarea"
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Incluye columnas de id, indicadores, nombre, duración, inicio y fin de la tarea.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Valor devuelto

una vista que contiene una lista de [`GanttChartColumn`](../../ganttchartcolumn/).

## Ejemplos

Muestra cómo guardar un proyecto con la vista de diagrama de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### Ver también

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


