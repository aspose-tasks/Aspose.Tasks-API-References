---
title: "Enum PdfPermissions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.PdfPermissions. Menentukan izin yang digunakan untuk mengakses dokumen PDF"
type: docs
weight: 2120
url: /id/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Menentukan izin yang digunakan untuk mengakses dokumen PDF.

```csharp
public enum PdfPermissions
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `0` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| Printing | `4` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| ModifyContents | `8` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| ContentCopy | `16` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| ModifyAnnotations | `32` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| FillIn | `256` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| ContentCopyForAccessibility | `512` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| DocumentAssembly | `1024` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| HighResolutionPrinting | `2052` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |
| AllowAll | `65535` | Menentukan izin yang digunakan untuk mengakses dokumen PDF. |

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


