---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PdfSaveOptions. يهيئ مثيلاً جديداً من فئة PdfSaveOptions يمكن استخدامه لحفظ مستند بتنسيق PDF"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

يهيئ مثيلاً جديداً من الفئة [`PdfSaveOptions`](../) التي يمكن استخدامها لحفظ مستند بتنسيق [`PDF`](../../savefileformat/).

```csharp
public PdfSaveOptions()
```

## الأمثلة

يوضح كيفية حفظ الصفحات المختارة لمشروع في ملف PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// دعنا نتحقق من عدد الصفحات التي يمكن تصديرها
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


