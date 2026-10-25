---
title: "SaveOptions.PresentationFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece el PresentationFormat en el que se guardará el documento"
type: docs
weight: 140
url: /es/net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

Obtiene o establece el `PresentationFormat` en el que se guardará el documento.

```csharp
public PresentationFormat PresentationFormat { get; set; }
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

Muestra cómo renderizar la vista de uso de tareas con la configuración de escala de tiempo definida en la configuración de la vista.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Defina las SaveOptions y especifique que se deben usar los ajustes de escala de tiempo de TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Ver también

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


