---
title: "SaveOptions.RollUpGanttBars"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece un valor que indica si las subtareas en la barra de tarea resumida deben marcarse. Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumida. Para las tareas resumidas, el campo Rollup indica si la barra de tarea resumida muestra barras consolidadas. Debe tener el campo Rollup de las tareas resumidas configurado en Sí para que cualquier subtarea se consolide en ellas."
type: docs
weight: 160
url: /es/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Obtiene o establece un valor que indica si las subtareas en la barra de tarea resumida deben marcarse. Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumida. Para las tareas resumidas, el campo Rollup indica si la barra de tarea resumida muestra barras consolidadas. Debe tener el campo Rollup de las tareas resumidas configurado en Yes para que cualquier subtarea se consolide en ellas.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Observaciones

Solo se aplica cuando se renderiza la vista de diagrama de Gantt.

## Ejemplos

Muestra cómo establecer un valor que indica que las subtareas en la barra de la tarea resumen deben consolidarse.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // O
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


