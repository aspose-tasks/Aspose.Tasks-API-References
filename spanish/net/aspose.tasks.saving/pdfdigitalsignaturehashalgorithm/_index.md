---
title: "Enumeración PdfDigitalSignatureHashAlgorithm"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. Especifica el algoritmo de hash digital utilizado por la firma digital"
type: docs
weight: 2090
url: /es/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Especifica el algoritmo de hash digital utilizado por la firma digital.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Sha1 | `0` | Especifica un algoritmo de hash digital utilizado por una firma digital. |
| Sha256 | `1` | Especifica un algoritmo de hash digital utilizado por una firma digital. |
| Sha384 | `2` | Especifica un algoritmo de hash digital utilizado por una firma digital. |
| Sha512 | `3` | Especifica un algoritmo de hash digital utilizado por una firma digital. |
| Md5 | `4` | Especifica un algoritmo de hash digital utilizado por una firma digital. |

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


