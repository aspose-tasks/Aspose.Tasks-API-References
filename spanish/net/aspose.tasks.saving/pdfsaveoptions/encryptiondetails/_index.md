---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece los detalles de cifrado. Si no se establece, no se realizará ningún cifrado."
type: docs
weight: 40
url: /es/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Obtiene o establece los detalles de cifrado. Si no se establece, no se realizará ningún cifrado.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Ejemplos

Muestra cómo establecer los detalles de cifrado de un documento PDF. Si no se establece, no se realizará ningún cifrado.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// establece los detalles de cifrado de un documento PDF
options.EncryptionDetails = encryptionDetails;

// ajustar propiedades adicionales
// establecer el <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> en el que se guardará el documento.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### Ver también

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


