---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PdfDigitalSignatureDetails. Initialise une nouvelle instance de la classe PdfDigitalSignatureDetails"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Initialise une nouvelle instance de la classe [`PdfDigitalSignatureDetails`](../).

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| certificat | X509Certificate2 | L'instance X509Certificate2 avec laquelle signer. |
| raison | Chaîne | La raison de la signature. |
| emplacement | Chaîne | Le lieu de la signature. |
| signatureDate | DateTime | La date de la signature. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | L'algorithme de hachage de la signature. |

## Exemples

Montre comment travailler avec les détails de la signature numérique PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// créer les détails de la signature PDF
var signatureDetails = new PdfDigitalSignatureDetails(
    // spécifier le certificat
    certificate, 
    // spécifier une raison de la signature
    "reason",
    // spécifier un lieu de signature
    "location", 
    // spécifier une date de signature
    new DateTime(2019, 1, 1), 
    // spécifier un algorithme de hachage de la signature
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// définir les détails de la signature numérique
options.DigitalSignatureDetails = signatureDetails;

// enregistrer le projet avec les détails de chiffrement spécifiés
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Voir aussi

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


