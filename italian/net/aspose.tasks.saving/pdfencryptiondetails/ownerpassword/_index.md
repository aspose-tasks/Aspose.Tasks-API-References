---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PdfEncryptionDetails. Ottiene o imposta la password Owner"
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

Ottiene o imposta la password del proprietario.

```csharp
public string OwnerPassword { get; set; }
```

## Osservazioni

Aprire il documento con la password proprietario corretta (supponendo che non sia la stessa della password utente) consente l'accesso completo (proprietario) al documento. Questo accesso illimitato include la possibilità di modificare le password del documento e le autorizzazioni di accesso.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


