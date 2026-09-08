---
title: "Enumeración PdfCompliance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Saving.PdfCompliance. Especifica el nivel de cumplimiento PDF para el archivo de salida"
type: docs
weight: 2070
url: /es/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Especifica el nivel de cumplimiento PDF para el archivo de salida.

```csharp
public enum PdfCompliance
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Pdf15 | `0` | Nivel de cumplimiento PDF/15. |
| PdfA1a | `1` | Nivel de cumplimiento PDF/A-1a. |
| PdfA1b | `2` | Nivel de cumplimiento PDF/A-1b. |

## Ejemplos

Muestra cómo establecer un nivel de cumplimiento deseado para el documento PDF generado.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// establecer un nivel de conformidad deseado para el documento PDF generado
// el valor predeterminado es <see cref=\"PdfCompliance.Pdf15\"/> tipo
options.Compliance = PdfCompliance.PdfA1b;

// ajustar propiedades adicionales
// establecer el <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> en el que se guardará el documento.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


