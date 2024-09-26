---
title: PdfDigitalSignatureDetails.Certificate
second_title: Aspose.Tasks for .NET API Reference
description: PdfDigitalSignatureDetails property. Gets or sets the certificate to sign with
type: docs
weight: 20
url: /net/aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/
---
## PdfDigitalSignatureDetails.Certificate property

Gets or sets the certificate to sign with.

```csharp
public X509Certificate2 Certificate { get; set; }
```

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

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


