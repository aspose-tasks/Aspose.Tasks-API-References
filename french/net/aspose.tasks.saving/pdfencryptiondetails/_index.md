---
title: "Classe PdfEncryptionDetails"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Saving.PdfEncryptionDetails. Contient les détails d'un chiffrement PDF"
type: docs
weight: 2110
url: /fr/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

Contient les détails d'un chiffrement PDF.

```csharp
public class PdfEncryptionDetails
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | Initialise une nouvelle instance de la classe `PdfEncryptionDetails`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | Obtient ou définit le mode de chiffrement. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | Obtient ou définit le mot de passe Owner. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | Obtient ou définit les autorisations. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | Obtient ou définit le mot de passe User. |

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


