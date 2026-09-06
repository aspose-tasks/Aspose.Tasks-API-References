---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعين الدقة الأفقية بوحدة dpi"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

يحصل أو يعيّن الدقة الأفقية بوحدة dpi.

```csharp
public float HorizontalResolution { get; set; }
```

## الأمثلة

يوضح كيفية تعيين تنسيق البكسل المستخدم أثناء التحويل إلى صيغ الصور.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### انظر أيضًا

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


