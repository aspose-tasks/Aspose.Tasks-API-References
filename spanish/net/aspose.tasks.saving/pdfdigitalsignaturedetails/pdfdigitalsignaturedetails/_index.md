---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor PdfDigitalSignatureDetails. Inicializa una nueva instancia de la clase PdfDigitalSignatureDetails"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Inicializa una nueva instancia de la clase [`PdfDigitalSignatureDetails`](../).

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| certificado | X509Certificate2 | La instancia X509Certificate2 con la que firmar. |
| razón | Cadena | La razón de la firma. |
| ubicación | Cadena | La ubicación de la firma. |
| signatureDate | DateTime | La fecha de la firma. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | El algoritmo hash de la firma. |

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


