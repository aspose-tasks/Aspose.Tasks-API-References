---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PdfDigitalSignatureDetails. يهيئ نسخة جديدة من فئة PdfDigitalSignatureDetails"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

يهيئ نسخة جديدة من الفئة [`PdfDigitalSignatureDetails`](../).

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| شهادة | X509Certificate2 | مثيل X509Certificate2 للتوقيع به. |
| السبب | سلسلة | السبب في التوقيع. |
| الموقع | سلسلة | الموقع الخاص بالتوقيع. |
| signatureDate | DateTime | تاريخ التوقيع. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | خوارزمية التجزئة للتوقيع. |

## الأمثلة

يوضح كيفية العمل مع تفاصيل التوقيع الرقمي PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// إنشاء تفاصيل توقيع PDF
var signatureDetails = new PdfDigitalSignatureDetails(
    // تحديد الشهادة
    certificate, 
    // تحديد سبب التوقيع
    "reason",
    // تحديد موقع التوقيع
    "location", 
    // تحديد تاريخ التوقيع
    new DateTime(2019, 1, 1), 
    // تحديد خوارزمية التجزئة للتوقيع
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// تعيين تفاصيل التوقيع الرقمي
options.DigitalSignatureDetails = signatureDetails;

// احفظ المشروع مع تفاصيل التشفير المحددة
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### انظر أيضًا

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


