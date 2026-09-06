---
title: "ImageSaveOptions.VerticalResolution"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعيين الدقة العمودية بوحدة dpi"
type: docs
weight: 100
url: /ar/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

يحصل أو يعيّن الدقة العمودية بوحدة dpi.

```csharp
public float VerticalResolution { get; set; }
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


