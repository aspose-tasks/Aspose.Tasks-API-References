---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectView. Incluye columnas de tarea con indicadores de id, nombre, duración, inicio, fin, predecesores y nombres de recursos"
type: docs
weight: 60
url: /es/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Incluye id, indicators, name, duration, start, finish, predecessors y columnas de tarea de nombres de recurso.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Valor devuelto

una vista que contiene una lista de [`GanttChartColumn`](../../ganttchartcolumn/).

## Ejemplos

Muestra cómo guardar un proyecto con la vista de hoja de tareas.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### Ver también

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


