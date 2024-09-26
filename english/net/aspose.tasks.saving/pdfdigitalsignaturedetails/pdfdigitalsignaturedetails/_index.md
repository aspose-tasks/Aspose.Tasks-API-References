---
title: PdfDigitalSignatureDetails.PdfDigitalSignatureDetails
second_title: Aspose.Tasks for .NET API Reference
description: PdfDigitalSignatureDetails constructor. Initializes a new instance of the PdfDigitalSignatureDetails class
type: docs
weight: 10
url: /net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Initializes a new instance of the [`PdfDigitalSignatureDetails`](../) class.

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parameter | Type | Description |
| --- | --- | --- |
| certificate | X509Certificate2 | The X509Certificate2 instance to sign with. |
| reason | String | The reason of signing. |
| location | String | The location of signing. |
| signatureDate | DateTime | The date of signing. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | The hash algorithm of signing. |

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

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


