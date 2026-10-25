---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore PdfDigitalSignatureDetails. Inizializza una nuova istanza della classe PdfDigitalSignatureDetails"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Inizializza una nuova istanza della classe [`PdfDigitalSignatureDetails`](../).

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| certificato | X509Certificate2 | L'istanza X509Certificate2 con cui firmare. |
| motivo | Stringa | Il motivo della firma. |
| posizione | Stringa | Il luogo della firma. |
| signatureDate | DateTime | La data della firma. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | L'algoritmo hash della firma. |

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

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


