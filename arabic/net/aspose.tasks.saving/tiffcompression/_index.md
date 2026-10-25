---
title: "تعداد TiffCompression"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Saving.TiffCompression. يحدد نوع الضغط الذي يجب تطبيقه عند حفظ الصفحات بتنسيق TIFF"
type: docs
weight: 2250
url: /ar/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

يحدد نوع الضغط الذي يتم تطبيقه عند حفظ الصفحات إلى تنسيق TIFF.

```csharp
public enum TiffCompression
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `1` | يحدد عدم وجود ضغط. |
| Rle | `2` | يحدد نظام ضغط RLE. |
| Ccitt3 | `3` | يحدد نظام ضغط CCITT3. |
| Ccitt4 | `4` | يحدد نظام ضغط CCITT4. |
| Lzw | `5` | يحدد نظام ضغط LZW. |

## الأمثلة

يوضح كيفية العرض بتنسيق TIFF باستخدام وضع ضغط RLE.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// احفظ المشروع باستخدام ضغط Rle
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


