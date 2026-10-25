---
title: "Enum PdfDigitalSignatureHashAlgorithm"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. Specificeert het digitale hash-algoritme dat wordt gebruikt door digitale handtekening"
type: docs
weight: 2090
url: /nl/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Bepaalt het digitale hash-algoritme dat wordt gebruikt door digitale handtekening.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Sha1 | `0` | Specificeert een digitaal hash-algoritme dat wordt gebruikt door een digitale handtekening. |
| Sha256 | `1` | Specificeert een digitaal hash-algoritme dat wordt gebruikt door een digitale handtekening. |
| Sha384 | `2` | Specificeert een digitaal hash-algoritme dat wordt gebruikt door een digitale handtekening. |
| Sha512 | `3` | Specificeert een digitaal hash-algoritme dat wordt gebruikt door een digitale handtekening. |
| Md5 | `4` | Specificeert een digitaal hash-algoritme dat wordt gebruikt door een digitale handtekening. |

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


