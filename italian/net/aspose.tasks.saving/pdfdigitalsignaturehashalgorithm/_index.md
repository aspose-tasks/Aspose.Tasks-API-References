---
title: "Enum PdfDigitalSignatureHashAlgorithm"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm. Specifica l'algoritmo di hash digitale utilizzato dalla firma digitale"
type: docs
weight: 2090
url: /it/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Specifica l'algoritmo di hash digitale utilizzato dalla firma digitale.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Sha1 | `0` | Specifica un algoritmo di hash digitale utilizzato da una firma digitale. |
| Sha256 | `1` | Specifica un algoritmo di hash digitale utilizzato da una firma digitale. |
| Sha384 | `2` | Specifica un algoritmo di hash digitale utilizzato da una firma digitale. |
| Sha512 | `3` | Specifica un algoritmo di hash digitale utilizzato da una firma digitale. |
| Md5 | `4` | Specifica un algoritmo di hash digitale utilizzato da una firma digitale. |

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


