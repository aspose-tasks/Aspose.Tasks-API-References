---
title: "Classe PdfEncryptionDetails"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.PdfEncryptionDetails. Contiene i dettagli per una crittografia PDF"
type: docs
weight: 2110
url: /it/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

Contiene i dettagli per una crittografia PDF.

```csharp
public class PdfEncryptionDetails
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | Inizializza una nuova istanza della classe `PdfEncryptionDetails`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | Ottiene o imposta la modalità di crittografia. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | Ottiene o imposta la password del proprietario. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | Ottiene o imposta le autorizzazioni. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | Ottiene o imposta la password dell'utente. |

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


