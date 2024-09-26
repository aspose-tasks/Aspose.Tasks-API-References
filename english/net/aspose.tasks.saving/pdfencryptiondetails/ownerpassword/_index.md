---
title: PdfEncryptionDetails.OwnerPassword
second_title: Aspose.Tasks for .NET API Reference
description: PdfEncryptionDetails property. Gets or sets the Owner password
type: docs
weight: 30
url: /net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

Gets or sets the Owner password.

```csharp
public string OwnerPassword { get; set; }
```

## Remarks

Opening the document with the correct owner password (assuming it is not the same as the user password) allows full (owner) access to the document. This unlimited access includes the ability to change the document’s passwords and access permissions.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


