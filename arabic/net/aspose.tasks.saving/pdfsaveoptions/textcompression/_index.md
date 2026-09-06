---
title: "PdfSaveOptions.TextCompression"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيين نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. الافتراضي هو Flate"
type: docs
weight: 100
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

يحصل أو يعيّن نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. القيمة الافتراضية هي Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## الأمثلة

يظهر كيفية تعيين نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// تعيين نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور
options.TextCompression = PdfTextCompression.Flate;

// ضبط الخصائص الإضافية
// تعيين <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> الذي سيُحفظ فيه المستند.
options.PresentationFormat = PresentationFormat.GanttChart;

// تعيين مستوى التوافق المطلوب للمستند PDF المُنشأ
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### انظر أيضًا

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


