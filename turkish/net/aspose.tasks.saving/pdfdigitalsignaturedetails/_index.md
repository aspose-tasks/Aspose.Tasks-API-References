---
title: "Sınıf PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureDetails sınıfı. PDF dijital imzası için ayrıntıları içerir."
type: docs
weight: 2080
url: /tr/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

PDF dijital imzası için ayrıntılar içerir.

```csharp
public class PdfDigitalSignatureDetails
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Yeni bir `PdfDigitalSignatureDetails` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | İmzalamak için kullanılacak sertifikayı alır veya ayarlar. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Karma algoritmasını alır veya ayarlar. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | İmza konumunu alır veya ayarlar. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | İmza nedenini alır veya ayarlar. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | İmza tarihini alır veya ayarlar. |

## Açıklamalar

Şu anda PDF belgelerini dijital olarak imzalama yalnızca .NET 2.0 veya üzeri sürümlerde mevcuttur.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


