---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PdfDigitalSignatureDetails. Menginisialisasi instance baru dari kelas PdfDigitalSignatureDetails"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Menginisialisasi instance baru dari kelas [`PdfDigitalSignatureDetails`](../).

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sertifikat | X509Certificate2 | Instance X509Certificate2 untuk menandatangani. |
| reason | String | Alasan penandatanganan. |
| location | String | Lokasi penandatanganan. |
| signatureDate | DateTime | Tanggal penandatanganan. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | Algoritma hash penandatanganan. |

## Contoh

Menampilkan cara bekerja dengan detail tanda tangan digital PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// buat detail tanda tangan PDF
var signatureDetails = new PdfDigitalSignatureDetails(
    // tentukan sertifikat
    certificate, 
    // tentukan alasan penandatanganan
    "reason",
    // tentukan lokasi penandatanganan
    "location", 
    // tentukan tanggal penandatanganan
    new DateTime(2019, 1, 1), 
    // tentukan algoritma hash penandatanganan
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// atur detail tanda tangan digital
options.DigitalSignatureDetails = signatureDetails;

// simpan proyek dengan detail enkripsi yang ditentukan
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Lihat Juga

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


