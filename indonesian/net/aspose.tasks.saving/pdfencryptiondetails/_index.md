---
title: "Kelas PdfEncryptionDetails"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.PdfEncryptionDetails. Berisi detail untuk enkripsi PDF"
type: docs
weight: 2110
url: /id/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

Berisi detail untuk enkripsi PDF.

```csharp
public class PdfEncryptionDetails
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | Menginisialisasi sebuah instance baru dari kelas `PdfEncryptionDetails`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | Mendapatkan atau mengatur mode enkripsi. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | Mendapatkan atau mengatur kata sandi Owner. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | Mendapatkan atau mengatur izin. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | Mendapatkan atau mengatur kata sandi User. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


