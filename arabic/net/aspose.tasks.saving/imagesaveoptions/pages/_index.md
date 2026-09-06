---
title: "ImageSaveOptions.Pages"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعين قائمة أرقام الصفحات التي تُحفظ عند حفظ تخطيط المشروع إلى ملفات منفصلة. سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة."
type: docs
weight: 50
url: /ar/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

يحصل أو يعيّن قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة. سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة.

```csharp
public List<int> Pages { get; set; }
```

## الأمثلة

يوضح كيفية حفظ الصفحات المحددة كصورة.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### انظر أيضًا

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


