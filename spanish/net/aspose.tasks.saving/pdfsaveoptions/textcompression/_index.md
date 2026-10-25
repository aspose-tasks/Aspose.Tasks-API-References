---
title: "PdfSaveOptions.TextCompression"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece un tipo de compresión que se usará para todos los flujos de contenido, excepto imágenes. El valor predeterminado es Flate"
type: docs
weight: 100
url: /es/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Obtiene o establece el tipo de compresión que se usará para todos los flujos de contenido, excepto imágenes. El valor predeterminado es Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## Ejemplos

Muestra cómo establecer un tipo de compresión que se usará para todas las secuencias de contenido, excepto las imágenes.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// establecer el tipo de compresión que se usará para todas las secuencias de contenido, excepto las imágenes
options.TextCompression = PdfTextCompression.Flate;

// ajustar propiedades adicionales
// establecer el <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> en el que se guardará el documento.
options.PresentationFormat = PresentationFormat.GanttChart;

// establecer un nivel de conformidad deseado para el documento PDF generado
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### Ver también

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


