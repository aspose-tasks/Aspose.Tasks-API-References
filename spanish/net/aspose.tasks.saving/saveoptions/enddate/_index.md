---
title: "SaveOptions.EndDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece una fecha para terminar la renderización."
type: docs
weight: 40
url: /es/net/aspose.tasks.saving/saveoptions/enddate/
---
## SaveOptions.EndDate property

Obtiene o establece una fecha para finalizar la renderización.

```csharp
public DateTime EndDate { get; set; }
```

## Ejemplos

Muestra cómo guardar el diseño en archivos separados.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Guardar el diseño del proyecto en archivos separados
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


