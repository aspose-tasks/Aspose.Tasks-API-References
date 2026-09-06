---
title: "SaveOptions.CustomPageSize"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد حجم الصفحة المخصص بالنقاط (1 نقطة = 1/72 بوصة)."
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

يحصل أو يعيّن حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 بوصة).

```csharp
public SizeF CustomPageSize { get; set; }
```

## الأمثلة

يوضح كيفية تعيين حجم الصفحة المخصص عند حفظ المشروع بصيغة PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


