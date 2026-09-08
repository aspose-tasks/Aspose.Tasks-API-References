---
title: "PdfDigitalSignatureDetails.Reason"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfDigitalSignatureDetails-eigenschap. Haalt op of stelt de reden van ondertekening in"
type: docs
weight: 50
url: /nl/net/aspose.tasks.saving/pdfdigitalsignaturedetails/reason/
---
## PdfDigitalSignatureDetails.Reason property

Haalt de reden van ondertekening op of stelt deze in.

```csharp
public string Reason { get; set; }
```

## Voorbeelden

Toont hoe te werken met PDF-digitaalhandtekeningdetails.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// maak PDF-handtekeningdetails
var signatureDetails = new PdfDigitalSignatureDetails(
    // specificeer certificaat
    certificate, 
    // specificeer een reden voor ondertekening
    "reason",
    // specificeer een locatie voor ondertekening
    "location", 
    // specificeer een datum voor ondertekening
    new DateTime(2019, 1, 1), 
    // specificeer een hash-algoritme voor ondertekening
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// stel digitale handtekeningdetails in
options.DigitalSignatureDetails = signatureDetails;

// sla het project op met gespecificeerde versleutelingsdetails
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Zie ook

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


