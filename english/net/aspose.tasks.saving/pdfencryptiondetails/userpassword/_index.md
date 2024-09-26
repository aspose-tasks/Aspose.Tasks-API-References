---
title: PdfEncryptionDetails.UserPassword
second_title: Aspose.Tasks for .NET API Reference
description: PdfEncryptionDetails property. Gets or sets the User password
type: docs
weight: 50
url: /net/aspose.tasks.saving/pdfencryptiondetails/userpassword/
---
## PdfEncryptionDetails.UserPassword property

Gets or sets the User password.

```csharp
public string UserPassword { get; set; }
```

## Remarks

Opening the document with the correct user password (or opening a document that does not have a user password) allows additional operations to be performed according to the user access permissions specified in the document’s encryption dictionary.

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


