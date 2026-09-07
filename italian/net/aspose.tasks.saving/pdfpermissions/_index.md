---
title: "Enum PdfPermissions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Saving.PdfPermissions. Specifica le autorizzazioni da utilizzare per accedere a un documento PDF"
type: docs
weight: 2120
url: /it/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Specifica le autorizzazioni da utilizzare per accedere a un documento PDF.

```csharp
public enum PdfPermissions
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| Printing | `4` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| ModifyContents | `8` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| ContentCopy | `16` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| ModifyAnnotations | `32` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| FillIn | `256` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| ContentCopyForAccessibility | `512` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| DocumentAssembly | `1024` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| HighResolutionPrinting | `2052` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |
| AllowAll | `65535` | Specifica le autorizzazioni da utilizzare per accedere a un documento PDF. |

## Esempi

Mostra come specificare i dettagli di crittografia PDF durante il salvataggio di un progetto come file PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// specifichiamo i dettagli di crittografia
var encryptionDetails = new PdfEncryptionDetails(
    // specifica la password dell'utente
    "userPassword", 
    // specifica la password del proprietario
    "ownerPassword", 
    // specifica l'algoritmo di crittografia
    PdfEncryptionAlgorithm.RC4_128);

// specifica le autorizzazioni
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// mostra le password dell'utente e del proprietario
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// mostra la modalità di crittografia: RC4_40 o RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// salva il progetto con i dettagli di crittografia specificati
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Vedi anche

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


