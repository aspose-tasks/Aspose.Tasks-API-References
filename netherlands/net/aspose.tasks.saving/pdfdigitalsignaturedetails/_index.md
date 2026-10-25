---
title: "Class PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureDetails class. Bevat details voor een digitale PDF-handtekening"
type: docs
weight: 2080
url: /nl/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Bevat details voor een digitale PDF‑handtekening.

```csharp
public class PdfDigitalSignatureDetails
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Initialiseert een nieuw exemplaar van de `PdfDigitalSignatureDetails`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Haalt het certificaat op of stelt het in waarmee ondertekend wordt. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Haalt de hash-algoritme op of stelt het in. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Haalt de locatie van ondertekening op of stelt deze in. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Haalt de reden van ondertekening op of stelt deze in. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Haalt de datum van ondertekening op of stelt deze in. |

## Opmerkingen

Op dit moment is digitaal ondertekenen van PDF-documenten alleen beschikbaar op .NET 2.0 of hoger.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


