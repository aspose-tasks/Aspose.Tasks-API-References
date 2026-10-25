---
title: "Clase PdfDigitalSignatureDetails"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.PdfDigitalSignatureDetails. Contiene detalles para una firma digital PDF"
type: docs
weight: 2080
url: /es/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Contiene detalles de una firma digital PDF.

```csharp
public class PdfDigitalSignatureDetails
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Inicializa una nueva instancia de la clase `PdfDigitalSignatureDetails`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Obtiene o establece el certificado con el que firmar. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Obtiene o establece el algoritmo de hash. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Obtiene o establece la ubicación de la firma. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Obtiene o establece la razón de la firma. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Obtiene o establece la fecha de la firma. |

## Observaciones

En este momento, la firma digital de documentos PDF solo está disponible en .NET 2.0 o superior.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


