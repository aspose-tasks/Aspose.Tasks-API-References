---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية XpsOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب عرض ملف ميتا كصورة نقطية."
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض ملف ميتا كصورة نقطية.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## الأمثلة

يوضح كيفية حفظ المشروع كملف XPS.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// إنشاء خيارات حفظ XPS وضبط المعلمات
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### انظر أيضًا

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


