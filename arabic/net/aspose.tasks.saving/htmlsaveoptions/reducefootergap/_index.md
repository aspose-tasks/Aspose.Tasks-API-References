---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية HtmlSaveOptions. يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة والتذييل"
type: docs
weight: 150
url: /ar/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

```csharp
public bool ReduceFooterGap { get; set; }
```

## الأمثلة

يوضح كيفية ضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة والتذييل في ملفات إخراج HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


