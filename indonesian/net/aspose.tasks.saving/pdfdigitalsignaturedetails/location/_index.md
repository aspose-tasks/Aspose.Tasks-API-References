---
title: "PdfDigitalSignatureDetails.Location"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfDigitalSignatureDetails. Mendapatkan atau mengatur lokasi penandatanganan"
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/pdfdigitalsignaturedetails/location/
---
## PdfDigitalSignatureDetails.Location property

Mendapatkan atau mengatur lokasi penandatanganan.

```csharp
public string Location { get; set; }
```

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

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


