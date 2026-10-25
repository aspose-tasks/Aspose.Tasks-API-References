---
title: "Enum PdfEncryptionAlgorithm"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PdfEncryptionAlgorithm enum. Specificeert het versleutelingsalgoritme dat gebruikt wordt om een PDF-document te versleutelen"
type: docs
weight: 2100
url: /nl/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

Bepaalt het encryptie-algoritme dat moet worden gebruikt voor het versleutelen van een PDF-document.

```csharp
public enum PdfEncryptionAlgorithm
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| RC4_40 | `0` | Bepaalt het encryptie-algoritme dat moet worden gebruikt voor het versleutelen van een PDF-document. |
| RC4_128 | `1` | Bepaalt het encryptie-algoritme dat moet worden gebruikt voor het versleutelen van een PDF-document. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


