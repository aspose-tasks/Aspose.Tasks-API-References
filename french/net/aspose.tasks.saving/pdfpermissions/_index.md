---
title: "Enum PdfPermissions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.Saving.PdfPermissions. Spécifie les autorisations à utiliser pour accéder à un document PDF"
type: docs
weight: 2120
url: /fr/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Spécifie les autorisations à utiliser pour accéder à un document PDF.

```csharp
public enum PdfPermissions
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| Printing | `4` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| ModifyContents | `8` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| ContentCopy | `16` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| ModifyAnnotations | `32` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| FillIn | `256` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| ContentCopyForAccessibility | `512` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| DocumentAssembly | `1024` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| HighResolutionPrinting | `2052` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |
| AllowAll | `65535` | Spécifie les autorisations à utiliser pour accéder à un document PDF. |

## Exemples

Montre comment spécifier les détails de chiffrement PDF lors de l'enregistrement d'un projet en fichier PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// spécifions les détails de chiffrement
var encryptionDetails = new PdfEncryptionDetails(
    // spécifier le mot de passe User
    "userPassword", 
    // spécifier le mot de passe Owner
    "ownerPassword", 
    // spécifier l'algorithme de chiffrement
    PdfEncryptionAlgorithm.RC4_128);

// spécifier les autorisations
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// afficher les mots de passe User et Owner
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// afficher le mode de chiffrement : RC4_40 ou RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// enregistrer le projet avec les détails de chiffrement spécifiés
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


