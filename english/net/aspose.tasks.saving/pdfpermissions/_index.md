---
title: Enum PdfPermissions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PdfPermissions enum. Specifies permissions to use for accessing a PDF document
type: docs
weight: 2100
url: /net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Specifies permissions to use for accessing a PDF document.

```csharp
public enum PdfPermissions
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Specifies permissions to use for accessing a PDF document. |
| Printing | `4` | Specifies permissions to use for accessing a PDF document. |
| ModifyContents | `8` | Specifies permissions to use for accessing a PDF document. |
| ContentCopy | `16` | Specifies permissions to use for accessing a PDF document. |
| ModifyAnnotations | `32` | Specifies permissions to use for accessing a PDF document. |
| FillIn | `256` | Specifies permissions to use for accessing a PDF document. |
| ContentCopyForAccessibility | `512` | Specifies permissions to use for accessing a PDF document. |
| DocumentAssembly | `1024` | Specifies permissions to use for accessing a PDF document. |
| HighResolutionPrinting | `2052` | Specifies permissions to use for accessing a PDF document. |
| AllowAll | `65535` | Specifies permissions to use for accessing a PDF document. |

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


