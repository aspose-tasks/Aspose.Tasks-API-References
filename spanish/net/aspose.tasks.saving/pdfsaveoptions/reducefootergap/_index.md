---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página."
type: docs
weight: 80
url: /es/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Obtiene o establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Ejemplos

Muestra cómo establecer un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página en los archivos PDF de salida.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


