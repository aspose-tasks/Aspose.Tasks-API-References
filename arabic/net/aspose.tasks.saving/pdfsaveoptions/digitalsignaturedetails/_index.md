---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيين تفاصيل التوقيع الرقمي. إذا لم يتم تعيينها فلن يتم تنفيذ أي توقيع"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

يحصل أو يعيّن تفاصيل التوقيع الرقمي. إذا لم يتم تعيينه، فلن يتم أي توقيع.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## الأمثلة

يوضح كيفية تعيين تفاصيل التوقيع الرقمي. إذا لم يتم تعيينها، فلن يتم تنفيذ أي توقيع.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// تعيين تفاصيل التوقيع الرقمي. إذا لم يتم تعيينها، فلن يتم تنفيذ أي توقيع.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// ضبط الخصائص الإضافية
// تعيين <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> الذي سيُحفظ فيه المستند.
options.PresentationFormat = PresentationFormat.GanttChart;

// تعيين مستوى التوافق المطلوب للمستند PDF المُنشأ
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### انظر أيضًا

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


