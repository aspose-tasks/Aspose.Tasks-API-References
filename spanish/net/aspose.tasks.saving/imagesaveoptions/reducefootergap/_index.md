---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página."
type: docs
weight: 80
url: /es/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Obtiene o establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Ejemplos

Muestra cómo establecer un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Use la propiedad ReduceFooterGap para reducir el espacio entre la lista de tareas y el pie de página.
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### Ver también

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


