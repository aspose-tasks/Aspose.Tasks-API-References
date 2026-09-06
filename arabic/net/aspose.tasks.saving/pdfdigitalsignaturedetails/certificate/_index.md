---
title: "PdfDigitalSignatureDetails.Certificate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfDigitalSignatureDetails. يحصل أو يضبط الشهادة المستخدمة للتوقيع"
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/
---
## PdfDigitalSignatureDetails.Certificate property

يحصل أو يضبط الشهادة المستخدمة للتوقيع.

```csharp
public X509Certificate2 Certificate { get; set; }
```

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

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


