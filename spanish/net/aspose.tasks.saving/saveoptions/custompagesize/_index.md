---
title: "SaveOptions.CustomPageSize"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada)."
type: docs
weight: 20
url: /es/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Ejemplos

Muestra cómo establecer el tamaño de página personalizado cuando el proyecto se guarda en PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


