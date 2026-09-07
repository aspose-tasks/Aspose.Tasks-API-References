---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PdfEncryptionDetails. Menginisialisasi sebuah instance baru dari kelas PdfEncryptionDetails"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

Menginisialisasi sebuah instance baru dari kelas [`PdfEncryptionDetails`](../).

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| `userPassword` | String | Password pengguna yang memungkinkan membuka dokumen yang dilindungi. |
| `ownerPassword` | String | Password pemilik yang memungkinkan membuka dokumen yang dilindungi. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | Instansi [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) yang menunjukkan algoritma enkripsi. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


