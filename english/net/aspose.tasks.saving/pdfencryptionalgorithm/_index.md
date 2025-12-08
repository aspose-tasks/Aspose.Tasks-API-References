---
title: Enum PdfEncryptionAlgorithm
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PdfEncryptionAlgorithm enum. Specifies the encryption algorithm to use for encrypting a PDF document
type: docs
weight: 2070
url: /net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

Specifies the encryption algorithm to use for encrypting a PDF document.

```csharp
public enum PdfEncryptionAlgorithm
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| RC4_40 | `0` | Specifies the encryption algorithm to use for encrypting a PDF document. |
| RC4_128 | `1` | Specifies the encryption algorithm to use for encrypting a PDF document. |

## Examples

Shows how to use specify PDF encryption details while saving a project as PDF file.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// lets specify encryption details  
var encryptionDetails = new PdfEncryptionDetails(
    // specify user password
    "userPassword", 
    // specify owner password
    "ownerPassword", 
    // specify encryption algorithm
    PdfEncryptionAlgorithm.RC4_128);

// specify permissions
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// show user and owner passwords
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// show encryption mode: RC4_40 or RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// save the project with specified encryption details
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


