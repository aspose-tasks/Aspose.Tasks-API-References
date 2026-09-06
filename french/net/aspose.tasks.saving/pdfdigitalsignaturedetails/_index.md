---
title: "Classe PdfDigitalSignatureDetails"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureDetails class. Contient les détails d'une signature numérique PDF"
type: docs
weight: 2080
url: /fr/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Contient les détails d'une signature numérique PDF.

```csharp
public class PdfDigitalSignatureDetails
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Initialise une nouvelle instance de la classe `PdfDigitalSignatureDetails`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Obtient ou définit le certificat avec lequel signer. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Obtient ou définit l'algorithme de hachage. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Obtient ou définit l'emplacement de la signature. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Obtient ou définit la raison de la signature. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Obtient ou définit la date de la signature. |

## Remarques

Pour le moment, la signature numérique de documents PDF n'est disponible que sur .NET 2.0 ou supérieur.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


