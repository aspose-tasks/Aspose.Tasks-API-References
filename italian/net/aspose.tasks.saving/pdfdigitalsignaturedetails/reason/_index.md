---
title: "PdfDigitalSignatureDetails.Reason"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PdfDigitalSignatureDetails. Ottiene o imposta il motivo della firma"
type: docs
weight: 50
url: /it/net/aspose.tasks.saving/pdfdigitalsignaturedetails/reason/
---
## PdfDigitalSignatureDetails.Reason property

Ottiene o imposta il motivo della firma.

```csharp
public string Reason { get; set; }
```

## Esempi

Mostra come lavorare con i dettagli della firma digitale PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// crea dettagli della firma PDF
var signatureDetails = new PdfDigitalSignatureDetails(
    // specifica il certificato
    certificate, 
    // specifica una motivazione della firma
    "reason",
    // specifica una posizione della firma
    "location", 
    // specifica una data della firma
    new DateTime(2019, 1, 1), 
    // specifica un algoritmo di hash della firma
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// imposta i dettagli della firma digitale
options.DigitalSignatureDetails = signatureDetails;

// salva il progetto con i dettagli di crittografia specificati
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Vedi anche

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


