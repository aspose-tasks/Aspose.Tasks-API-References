---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfDigitalSignatureDetails-constructor. Initialiseert een nieuw exemplaar van de PdfDigitalSignatureDetails-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Initialiseert een nieuw exemplaar van de [`PdfDigitalSignatureDetails`](../)-klasse.

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| certificaat | X509Certificate2 | De X509Certificate2-instantie om mee te ondertekenen. |
| reden | String | De reden van ondertekening. |
| locatie | String | De locatie van ondertekening. |
| ondertekeningsdatum | DateTime | De datum van ondertekening. |
| hashAlgoritme | PdfDigitalSignatureHashAlgorithm | Het hash-algoritme van ondertekening. |

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

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


