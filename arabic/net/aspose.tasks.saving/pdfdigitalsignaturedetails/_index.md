---
title: "فئة PdfDigitalSignatureDetails"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Saving.PdfDigitalSignatureDetails. تحتوي على تفاصيل توقيع PDF الرقمي"
type: docs
weight: 2080
url: /ar/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

يحتوي على تفاصيل لتوقيع PDF الرقمي.

```csharp
public class PdfDigitalSignatureDetails
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | يُنشئ مثلاً جديداً من الفئة `PdfDigitalSignatureDetails`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | يحصل أو يضبط الشهادة المستخدمة للتوقيع. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | يحصل أو يضبط خوارزمية التجزئة. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | يحصل أو يضبط موقع التوقيع. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | يحصل أو يضبط سبب التوقيع. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | يحصل أو يضبط تاريخ التوقيع. |

## ملاحظات

في الوقت الحالي، التوقيع الرقمي لمستندات PDF متاح فقط على .NET 2.0 أو أعلى.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


