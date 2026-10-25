---
title: "Enum PdfDigitalSignatureHashAlgorithm"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. Menentukan algoritma hash digital yang digunakan oleh tanda tangan digital."
type: docs
weight: 2090
url: /id/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Menentukan algoritma hash digital yang digunakan oleh tanda tangan digital.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Sha1 | `0` | Menentukan algoritma hash digital yang digunakan oleh tanda tangan digital. |
| Sha256 | `1` | Menentukan algoritma hash digital yang digunakan oleh tanda tangan digital. |
| Sha384 | `2` | Menentukan algoritma hash digital yang digunakan oleh tanda tangan digital. |
| Sha512 | `3` | Menentukan algoritma hash digital yang digunakan oleh tanda tangan digital. |
| Md5 | `4` | Menentukan algoritma hash digital yang digunakan oleh tanda tangan digital. |

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


