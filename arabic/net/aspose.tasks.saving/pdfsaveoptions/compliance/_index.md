---
title: "PdfSaveOptions.Compliance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيين مستوى الامتثال المطلوب للمستند PDF المُولد. الافتراضي هو Pdf15"
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

يحصل أو يعيّن مستوى الامتثال المطلوب للمستند PDF المُولَّد. القيمة الافتراضية هي Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


