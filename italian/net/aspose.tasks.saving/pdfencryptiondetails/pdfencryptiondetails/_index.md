---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore PdfEncryptionDetails. Inizializza una nuova istanza della classe PdfEncryptionDetails"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

Inizializza una nuova istanza della classe [`PdfEncryptionDetails`](../).

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| userPassword | Stringa | La password utente che consente di aprire documenti protetti. |
| ownerPassword | Stringa | La password proprietario che consente di aprire documenti protetti. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | L'istanza [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) che indica l'algoritmo di crittografia. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


