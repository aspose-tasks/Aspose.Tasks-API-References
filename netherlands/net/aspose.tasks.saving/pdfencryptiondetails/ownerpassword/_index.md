---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfEncryptionDetails eigenschap. Haalt op of stelt het eigenaarswachtwoord in."
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

Haalt op of stelt het eigenaarswachtwoord in.

```csharp
public string OwnerPassword { get; set; }
```

## Opmerkingen

Het openen van het document met het juiste eigenaarswachtwoord (ervan uitgaande dat dit niet hetzelfde is als het gebruikerswachtwoord) geeft volledige (eigenaars‑)toegang tot het document. Deze onbeperkte toegang omvat de mogelijkheid om de wachtwoorden van het document en de toegangsrechten te wijzigen.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


