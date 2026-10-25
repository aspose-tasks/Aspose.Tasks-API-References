---
title: "Enum PdfPermissions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PdfPermissions‑enum. Specificeert de rechten die gebruikt moeten worden voor toegang tot een PDF‑document."
type: docs
weight: 2120
url: /nl/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document.

```csharp
public enum PdfPermissions
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| Printing | `4` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| ModifyContents | `8` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| ContentCopy | `16` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| ModifyAnnotations | `32` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| FillIn | `256` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| ContentCopyForAccessibility | `512` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| DocumentAssembly | `1024` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| HighResolutionPrinting | `2052` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |
| AllowAll | `65535` | Bepaalt de machtigingen die moeten worden gebruikt voor het openen van een PDF-document. |

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


