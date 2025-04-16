---
title: Class PdfDigitalSignatureDetails
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PdfDigitalSignatureDetails class. Contains details for a PDF digital signature
type: docs
weight: 2020
url: /net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Contains details for a PDF digital signature.

```csharp
public class PdfDigitalSignatureDetails
```

## Constructors

| Name | Description |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Initializes a new instance of the `PdfDigitalSignatureDetails` class. |

## Properties

| Name | Description |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Gets or sets the certificate to sign with. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Gets or sets the hash algorithm. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Gets or sets the location of signing. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Gets or sets the reason of signing. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Gets or sets the date of signing. |

## Remarks

At the moment digitally signing PDF documents is only available on .NET 2.0 or higher.

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


