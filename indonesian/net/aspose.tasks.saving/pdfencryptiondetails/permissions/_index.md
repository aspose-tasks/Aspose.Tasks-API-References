---
title: "PdfEncryptionDetails.Permissions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfEncryptionDetails. Mendapatkan atau mengatur izin"
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/pdfencryptiondetails/permissions/
---
## PdfEncryptionDetails.Permissions property

Mendapatkan atau mengatur izin.

```csharp
public PdfPermissions Permissions { get; set; }
```

## Contoh

Menampilkan cara menggunakan detail enkripsi PDF saat menyimpan proyek sebagai file PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// mari tentukan detail enkripsi
var encryptionDetails = new PdfEncryptionDetails(
    // tentukan kata sandi user
    "userPassword", 
    // tentukan kata sandi owner
    "ownerPassword", 
    // tentukan algoritma enkripsi
    PdfEncryptionAlgorithm.RC4_128);

// tentukan izin
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// tampilkan kata sandi user dan owner
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// tampilkan mode enkripsi: RC4_40 atau RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// simpan proyek dengan detail enkripsi yang ditentukan
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Lihat Juga

* enum [PdfPermissions](../../pdfpermissions/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


