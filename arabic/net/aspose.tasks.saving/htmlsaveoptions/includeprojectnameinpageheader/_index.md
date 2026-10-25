---
title: "HtmlSaveOptions.IncludeProjectNameInPageHeader"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية HtmlSaveOptions. تحصل أو تعيين قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML"
type: docs
weight: 110
url: /ar/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/
---
## HtmlSaveOptions.IncludeProjectNameInPageHeader property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في ترويسة صفحة HTML.

```csharp
public bool IncludeProjectNameInPageHeader { get; set; }
```

## الأمثلة

يوضح كيفية تعيين رأس/عنوان صفحة HTML باستخدام خيارات &lt;see cref=\"P:Aspose.Tasks.Saving.HtmlSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // يحدد ما إذا كان يجب تضمين اسم المشروع في عنوان HTML (true بشكل افتراضي)
    IncludeProjectNameInTitle = false,

    // يحدد ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML (true بشكل افتراضي)
    IncludeProjectNameInPageHeader = false,

    // تعيين الصفحات التي سيتم تصديرها
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


