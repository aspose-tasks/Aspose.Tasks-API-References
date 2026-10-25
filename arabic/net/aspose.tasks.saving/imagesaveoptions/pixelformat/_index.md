---
title: "ImageSaveOptions.PixelFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعين تنسيق بيانات اللون لكل بكسل في الصورة."
type: docs
weight: 70
url: /ar/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

يحصل أو يعيّن تنسيق بيانات اللون لكل بكسل في الصورة.

```csharp
public PixelFormat PixelFormat { get; set; }
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


