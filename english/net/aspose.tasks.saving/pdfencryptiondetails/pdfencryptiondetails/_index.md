---
title: PdfEncryptionDetails.PdfEncryptionDetails
second_title: Aspose.Tasks for .NET API Reference
description: PdfEncryptionDetails constructor. Initializes a new instance of the PdfEncryptionDetails class
type: docs
weight: 10
url: /net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

Initializes a new instance of the [`PdfEncryptionDetails`](../) class.

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Parameter | Type | Description |
| --- | --- | --- |
| userPassword | String | The user password allowing to open protected documents. |
| ownerPassword | String | The owner password allowing to open protected documents. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | The [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) instance which indicate encryption algorithm. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


