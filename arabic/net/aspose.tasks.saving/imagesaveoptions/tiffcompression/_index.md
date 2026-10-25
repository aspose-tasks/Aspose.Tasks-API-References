---
title: "ImageSaveOptions.TiffCompression"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعين نوع الضغط الذي يُطبق عند حفظ الصور المُولدة بصيغة TIFF"
type: docs
weight: 90
url: /ar/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

يحصل أو يعيّن نوع الضغط الذي سيُطبق عند حفظ الصور المُولَّدة بتنسيق TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## ملاحظات

يؤثر فقط عند الحفظ بصيغة TIFF. القيمة الافتراضية هي `LZW`.

## الأمثلة

يوضح كيفية تعيين ضغط TIFF لملفات TIFF الناتجة.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// من أجل تعديل ضغط TIFF يمكننا استخدام خاصية ImageSaveOptions.TiffCompression.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### انظر أيضًا

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


