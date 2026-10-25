---
title: "PdfDigitalSignatureDetails.HashAlgorithm"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfDigitalSignatureDetails. Obtiene o establece el algoritmo hash"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/
---
## PdfDigitalSignatureDetails.HashAlgorithm property

Obtiene o establece el algoritmo de hash.

```csharp
public PdfDigitalSignatureHashAlgorithm HashAlgorithm { get; set; }
```

## Ejemplos

Muestra cómo trabajar con los detalles de la firma digital PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// crear detalles de firma PDF
var signatureDetails = new PdfDigitalSignatureDetails(
    // especificar certificado
    certificate, 
    // especificar una razón de la firma
    "reason",
    // especificar una ubicación de la firma
    "location", 
    // especificar una fecha de la firma
    new DateTime(2019, 1, 1), 
    // especificar un algoritmo de hash de la firma
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// establecer detalles de firma digital
options.DigitalSignatureDetails = signatureDetails;

// guardar el proyecto con los detalles de cifrado especificados
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Ver también

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


