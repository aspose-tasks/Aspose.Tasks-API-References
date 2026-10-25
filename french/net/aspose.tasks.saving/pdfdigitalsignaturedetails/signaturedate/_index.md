---
title: "PdfDigitalSignatureDetails.SignatureDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfDigitalSignatureDetails. Obtient ou définit la date de signature"
type: docs
weight: 60
url: /fr/net/aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/
---
## PdfDigitalSignatureDetails.SignatureDate property

Obtient ou définit la date de la signature.

```csharp
public DateTime SignatureDate { get; set; }
```

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

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


