---
title: "تعداد PdfCompliance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Saving.PdfCompliance. يحدد مستوى توافق PDF لملف الإخراج"
type: docs
weight: 2070
url: /ar/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

يحدد مستوى توافق PDF لملف الإخراج.

```csharp
public enum PdfCompliance
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Pdf15 | `0` | مستوى توافق PDF/15. |
| PdfA1a | `1` | مستوى توافق PDF/A-1a. |
| PdfA1b | `2` | مستوى توافق PDF/A-1b. |

## الأمثلة

يوضح كيفية ضبط مستوى توافق مطلوب للمستند PDF المُولد.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// تعيين مستوى التوافق المطلوب للمستند PDF المُنشأ
// الافتراضي هو النوع <see cref=\"PdfCompliance.Pdf15\"/>
options.Compliance = PdfCompliance.PdfA1b;

// ضبط الخصائص الإضافية
// تعيين <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> الذي سيُحفظ فيه المستند.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


