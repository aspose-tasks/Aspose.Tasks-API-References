---
title: "PdfDigitalSignatureDetails.Location"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfDigitalSignatureDetails özelliği. İmza konumunu alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks.saving/pdfdigitalsignaturedetails/location/
---
## PdfDigitalSignatureDetails.Location property

İmza konumunu alır veya ayarlar.

```csharp
public string Location { get; set; }
```

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

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


