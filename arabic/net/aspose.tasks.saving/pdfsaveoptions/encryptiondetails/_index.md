---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيين تفاصيل التشفير. إذا لم يتم تعيينها فلن يتم تنفيذ أي تشفير"
type: docs
weight: 40
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

يحصل أو يعيّن تفاصيل التشفير. إذا لم يتم تعيينه، فلن يتم أي تشفير.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## الأمثلة

يوضح كيفية تعيين تفاصيل التشفير لمستند PDF. إذا لم يتم تعيينها، فلن يتم تنفيذ أي تشفير.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// تعيين تفاصيل التشفير لمستند PDF
options.EncryptionDetails = encryptionDetails;

// ضبط الخصائص الإضافية
// تعيين <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> الذي سيُحفظ فيه المستند.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### انظر أيضًا

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


