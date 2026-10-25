---
title: "XpsOptions.XpsOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ XpsOptions. يهيئ مثيلاً جديداً لفئة XpsOptions"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

يهيئ مثيلاً جديداً لفئة [`XpsOptions`](../).

```csharp
public XpsOptions()
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


