---
title: "Kelas PdfDigitalSignatureDetails"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.PdfDigitalSignatureDetails. Berisi detail untuk tanda tangan digital PDF."
type: docs
weight: 2080
url: /id/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Berisi detail untuk tanda tangan digital PDF.

```csharp
public class PdfDigitalSignatureDetails
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Menginisialisasi instance baru dari kelas `PdfDigitalSignatureDetails`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Mendapatkan atau mengatur sertifikat untuk menandatangani. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Mendapatkan atau mengatur algoritma hash. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Mendapatkan atau mengatur lokasi penandatanganan. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Mendapatkan atau mengatur alasan penandatanganan. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Mendapatkan atau mengatur tanggal penandatanganan. |

## Catatan

Saat ini penandatanganan digital dokumen PDF hanya tersedia pada .NET 2.0 atau yang lebih tinggi.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


