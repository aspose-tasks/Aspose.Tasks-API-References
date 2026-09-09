---
title: "Enum PdfDigitalSignatureHashAlgorithm"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. Dijital imza tarafından kullanılan dijital hash algoritmasını belirtir"
type: docs
weight: 2090
url: /tr/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Dijital imza tarafından kullanılan dijital özet algoritmasını belirtir.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Sha1 | `0` | Dijital imza tarafından kullanılan bir dijital hash algoritmasını belirtir. |
| Sha256 | `1` | Dijital imza tarafından kullanılan bir dijital hash algoritmasını belirtir. |
| Sha384 | `2` | Dijital imza tarafından kullanılan bir dijital hash algoritmasını belirtir. |
| Sha512 | `3` | Dijital imza tarafından kullanılan bir dijital hash algoritmasını belirtir. |
| Md5 | `4` | Dijital imza tarafından kullanılan bir dijital hash algoritmasını belirtir. |

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


