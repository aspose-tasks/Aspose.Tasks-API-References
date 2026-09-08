---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece los detalles de la firma digital. Si no se establece, no se realizará ninguna firma."
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Obtiene o establece los detalles de la firma digital. Si no se establece, no se realizará ninguna firma.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Ejemplos

Muestra cómo establecer los detalles de la firma digital. Si no se establece, no se realizará ninguna firma.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// establece los detalles de la firma digital. Si no se establece, no se realizará ninguna firma.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// ajustar propiedades adicionales
// establecer el <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> en el que se guardará el documento.
options.PresentationFormat = PresentationFormat.GanttChart;

// establecer un nivel de conformidad deseado para el documento PDF generado
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### Ver también

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


