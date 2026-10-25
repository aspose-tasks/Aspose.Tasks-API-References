---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ HtmlSaveOptions. يهيئ نسخة جديدة من الفئة HtmlSaveOptions"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

يهيئ نسخة جديدة من الفئة [`HtmlSaveOptions`](../).

```csharp
public HtmlSaveOptions()
```

## الأمثلة

يوضح كيفية حفظ مشروع بتنسيق HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// أو

// إضافة صفحة واحدة فقط (رقم الصفحة 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


