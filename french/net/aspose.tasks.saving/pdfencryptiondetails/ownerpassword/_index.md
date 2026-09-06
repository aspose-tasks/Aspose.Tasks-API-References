---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfEncryptionDetails. Obtient ou définit le mot de passe propriétaire"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

Obtient ou définit le mot de passe Owner.

```csharp
public string OwnerPassword { get; set; }
```

## Remarques

Ouvrir le document avec le mot de passe propriétaire correct (en supposant qu'il ne soit pas identique au mot de passe utilisateur) permet un accès complet (propriétaire) au document. Cet accès illimité comprend la possibilité de modifier les mots de passe du document et les autorisations d'accès.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


