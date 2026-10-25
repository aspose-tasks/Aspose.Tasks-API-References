---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية HtmlSaveOptions. تحصل أو تعيين بادئة نمط CSS"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

يحصل أو يعيّن بادئة نمط CSS.

```csharp
public string CssStylePrefix { get; set; }
```

## الأمثلة

يوضح كيفية تعيين بادئة مشتركة لأنماط CSS المستخدمة أثناء التصدير إلى HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


