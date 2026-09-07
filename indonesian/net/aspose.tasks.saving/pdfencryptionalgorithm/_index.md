---
title: "Enum PdfEncryptionAlgorithm"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.PdfEncryptionAlgorithm. Menentukan algoritma enkripsi yang digunakan untuk mengenkripsi dokumen PDF"
type: docs
weight: 2100
url: /id/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

Menentukan algoritma enkripsi yang digunakan untuk mengenkripsi dokumen PDF.

```csharp
public enum PdfEncryptionAlgorithm
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| RC4_40 | `0` | Menentukan algoritma enkripsi yang digunakan untuk mengenkripsi dokumen PDF. |
| RC4_128 | `1` | Menentukan algoritma enkripsi yang digunakan untuk mengenkripsi dokumen PDF. |

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


