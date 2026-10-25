---
title: "SaveOptions.FitContent"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido."
type: docs
weight: 50
url: /es/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Obtiene o establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido.

```csharp
public bool FitContent { get; set; }
```

## Ejemplos

Muestra cómo establecer la opción de si la altura de la fila debe aumentarse para ajustarse a su contenido.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Establecer la opción ajustar contenido a true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


