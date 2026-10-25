---
title: "التعداد PdfTextCompression"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Saving.PdfTextCompression. يحدد نوع الضغط المطبق على جميع محتويات ملف PDF باستثناء الصور."
type: docs
weight: 2140
url: /ar/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

يحدد نوع الضغط المطبق على جميع محتويات ملف PDF باستثناء الصور.

```csharp
public enum PdfTextCompression
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون ضغط. |
| Flate | `1` | ضغط Flate. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


