---
title: "Enum PdfTextCompression"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.Saving.PdfTextCompression. Especifica un tipo de compresión aplicado a todo el contenido del archivo PDF, excepto a las imágenes."
type: docs
weight: 2140
url: /es/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Especifica un tipo de compresión aplicado a todo el contenido del archivo PDF, excepto a las imágenes.

```csharp
public enum PdfTextCompression
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin compresión. |
| Flate | `1` | Compresión Flate. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


