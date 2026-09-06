---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيين قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين آخر مهمة وتذييل الصفحة"
type: docs
weight: 80
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

```csharp
public bool ReduceFooterGap { get; set; }
```

## الأمثلة

يوضح كيفية تعيين قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين آخر مهمة وتذييل الصفحة في ملفات إخراج PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


