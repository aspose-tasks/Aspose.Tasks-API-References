---
title: "PdfSaveOptions.Pages"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيين قائمة أرقام الصفحات التي يجب حفظها عند حفظ تخطيط المشروع في ملفات منفصلة. سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة"
type: docs
weight: 60
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

يحصل أو يعيّن قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة. سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة.

```csharp
public List<int> Pages { get; set; }
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


