---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece un valor que indica si el tiempo no laborable debe dibujarse. El valor predeterminado es TRUE."
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Obtiene o establece un valor que indica si el tiempo no laborable debe dibujarse (El valor predeterminado es TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

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


