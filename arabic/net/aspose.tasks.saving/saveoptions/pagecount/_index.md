---
title: "SaveOptions.PageCount"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد عدد صفحات المشروع."
type: docs
weight: 120
url: /ar/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

يحصل أو يعيّن عدد صفحات المشروع.

```csharp
public int PageCount { get; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


