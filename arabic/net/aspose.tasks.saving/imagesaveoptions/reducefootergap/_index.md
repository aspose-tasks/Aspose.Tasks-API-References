---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة والتذييل."
type: docs
weight: 80
url: /ar/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

```csharp
public bool ReduceFooterGap { get; set; }
```

## الأمثلة

يوضح كيفية تعيين قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة والتذييل.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// استخدم خاصية ReduceFooterGap لتقليل الفجوة بين قائمة المهام والتذييل.
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### انظر أيضًا

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


