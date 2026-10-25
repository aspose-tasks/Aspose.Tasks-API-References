---
title: "HtmlSaveOptions.Pages"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية HtmlSaveOptions. تحصل أو تعيين قائمة بأرقام الصفحات لحفظها عند تصيير تخطيط المشروع. سيتم حفظ جميع صفحات المشروع إذا كانت هذه القائمة فارغة"
type: docs
weight: 130
url: /ar/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

يحصل أو يعيّن قائمة بأرقام الصفحات التي يجب حفظها عند عرض تخطيط المشروع. سيتم حفظ جميع صفحات المشروع إذا كانت هذه القائمة فارغة.

```csharp
public List<int> Pages { get; set; }
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


