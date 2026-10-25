---
title: "Class PdfDigitalSignatureDetails"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.PdfDigitalSignatureDetails. Contiene i dettagli per una firma digitale PDF"
type: docs
weight: 2080
url: /it/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Contiene i dettagli per una firma digitale PDF.

```csharp
public class PdfDigitalSignatureDetails
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Inizializza una nuova istanza della classe `PdfDigitalSignatureDetails`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Ottiene o imposta il certificato con cui firmare. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Ottiene o imposta l'algoritmo di hash. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Ottiene o imposta la posizione della firma. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Ottiene o imposta il motivo della firma. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Ottiene o imposta la data della firma. |

## Osservazioni

Al momento la firma digitale dei documenti PDF è disponibile solo su .NET 2.0 o versioni successive.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


