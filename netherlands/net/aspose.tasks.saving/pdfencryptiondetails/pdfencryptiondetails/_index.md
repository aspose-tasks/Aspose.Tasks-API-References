---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfEncryptionDetails constructor. Initialiseert een nieuwe instantie van de PdfEncryptionDetails klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

Initialiseert een nieuwe instantie van de [`PdfEncryptionDetails`](../) klasse.

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| userPassword | String | Het gebruikerswachtwoord dat het openen van beveiligde documenten mogelijk maakt. |
| ownerPassword | String | Het eigenaarswachtwoord dat het openen van beveiligde documenten mogelijk maakt. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | De [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) instantie die het encryptie‑algoritme aangeeft. |

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


