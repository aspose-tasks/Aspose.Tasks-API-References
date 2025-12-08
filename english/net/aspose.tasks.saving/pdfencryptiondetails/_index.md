---
title: Class PdfEncryptionDetails
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PdfEncryptionDetails class. Contains details for a PDF encryption
type: docs
weight: 2080
url: /net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

Contains details for a PDF encryption.

```csharp
public class PdfEncryptionDetails
```

## Constructors

| Name | Description |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | Initializes a new instance of the `PdfEncryptionDetails` class. |

## Properties

| Name | Description |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | Gets or sets the encryption mode. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | Gets or sets the Owner password. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | Gets or sets the permissions. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | Gets or sets the User password. |

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


