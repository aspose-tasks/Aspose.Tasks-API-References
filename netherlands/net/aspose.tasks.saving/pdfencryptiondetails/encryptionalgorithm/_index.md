---
title: "PdfEncryptionDetails.EncryptionAlgorithm"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfEncryptionDetails eigenschap. Haalt op of stelt de encryptiemodus in."
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/
---
## PdfEncryptionDetails.EncryptionAlgorithm property

Haalt op of stelt de versleutelingsmodus in.

```csharp
public PdfEncryptionAlgorithm EncryptionAlgorithm { get; set; }
```

## Voorbeelden

Toont hoe je PDF-versleutelingsdetails specificeert bij het opslaan van een project als PDF-bestand.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// laten we versleutelingsdetails specificeren
var encryptionDetails = new PdfEncryptionDetails(
    // specificeer gebruikerswachtwoord
    "userPassword", 
    // specificeer eigenaarswachtwoord
    "ownerPassword", 
    // specificeer versleutelingsalgoritme
    PdfEncryptionAlgorithm.RC4_128);

// specificeer permissies
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// toon gebruikers- en eigenaarswachtwoorden
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// toon versleutelingsmodus: RC4_40 of RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// sla het project op met gespecificeerde versleutelingsdetails
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Zie ook

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


