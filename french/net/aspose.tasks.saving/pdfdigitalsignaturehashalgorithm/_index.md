---
title: "Enum PdfDigitalSignatureHashAlgorithm"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. Spécifie l'algorithme de hachage numérique utilisé par la signature numérique"
type: docs
weight: 2090
url: /fr/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Spécifie l'algorithme de hachage numérique utilisé par la signature numérique.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Sha1 | `0` | Spécifie un algorithme de hachage numérique utilisé par une signature numérique. |
| Sha256 | `1` | Spécifie un algorithme de hachage numérique utilisé par une signature numérique. |
| Sha384 | `2` | Spécifie un algorithme de hachage numérique utilisé par une signature numérique. |
| Sha512 | `3` | Spécifie un algorithme de hachage numérique utilisé par une signature numérique. |
| Md5 | `4` | Spécifie un algorithme de hachage numérique utilisé par une signature numérique. |

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


