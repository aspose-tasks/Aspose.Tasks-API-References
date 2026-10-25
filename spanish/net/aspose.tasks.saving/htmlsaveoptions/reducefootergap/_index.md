---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página"
type: docs
weight: 150
url: /es/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Obtiene o establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Ejemplos

Muestra cómo establecer un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página en los archivos de salida HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


