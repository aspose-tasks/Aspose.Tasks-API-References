---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página."
type: docs
weight: 210
url: /es/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Obtiene o establece un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Ejemplos

Muestra cómo usar TimescaleFitBehavior para que la escala de tiempo del diagrama de Gantt se ajuste al final de la última página.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Ver también

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


