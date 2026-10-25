---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfDigitalSignatureDetails yapıcı. PdfDigitalSignatureDetails sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

[`PdfDigitalSignatureDetails`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sertifika | X509Certificate2 | İmzalamak için kullanılacak X509Certificate2 örneği. |
| reason | Dize | İmzalamanın nedeni. |
| location | Dize | İmzalamanın konumu. |
| signatureDate | DateTime | İmzalamanın tarihi. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | İmzalamanın hash algoritması. |

## Örnekler

PDF dijital imza detaylarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// PDF imza detaylarını oluştur
var signatureDetails = new PdfDigitalSignatureDetails(
    // sertifikayı belirt
    certificate, 
    // imzalama nedenini belirt
    "reason",
    // imzalama konumunu belirt
    "location", 
    // imzalama tarihini belirt
    new DateTime(2019, 1, 1), 
    // imzalama için bir hash algoritması belirt
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// dijital imza detaylarını ayarla
options.DigitalSignatureDetails = signatureDetails;

// belirtilen şifreleme ayrıntılarıyla projeyi kaydet
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Ayrıca Bakınız

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


