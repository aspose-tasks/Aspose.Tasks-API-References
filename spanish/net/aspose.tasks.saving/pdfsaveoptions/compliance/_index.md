---
title: "PdfSaveOptions.Compliance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece el nivel de cumplimiento deseado para el documento PDF generado. El valor predeterminado es Pdf15."
type: docs
weight: 20
url: /es/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Obtiene o establece el nivel de cumplimiento deseado para el documento PDF generado. El valor predeterminado es Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


