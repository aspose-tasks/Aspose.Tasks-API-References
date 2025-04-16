---
title: Enum PdfDigitalSignatureHashAlgorithm
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. Specifies digital hash algorithm used by digital signature
type: docs
weight: 2030
url: /net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Specifies digital hash algorithm used by digital signature.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Sha1 | `0` | Specifies a digital hash algorithm used by a digital signature. |
| Sha256 | `1` | Specifies a digital hash algorithm used by a digital signature. |
| Sha384 | `2` | Specifies a digital hash algorithm used by a digital signature. |
| Sha512 | `3` | Specifies a digital hash algorithm used by a digital signature. |
| Md5 | `4` | Specifies a digital hash algorithm used by a digital signature. |

## Examples

Shows how to work with PDF digital signature details.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// create PDF signature details
var signatureDetails = new PdfDigitalSignatureDetails(
    // specify certificate
    certificate, 
    // specify a reason of signing
    "reason",
    // specify a location of signing
    "location", 
    // specify a date of signing
    new DateTime(2019, 1, 1), 
    // specify a hash algorithm of signing
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// set digital signature details
options.DigitalSignatureDetails = signatureDetails;

// save the project with specified encryption details
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


