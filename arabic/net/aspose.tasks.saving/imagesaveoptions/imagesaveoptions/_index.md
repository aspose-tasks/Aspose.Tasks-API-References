---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ImageSaveOptions. يهيئ مثيلاً جديداً من فئة ImageSaveOptions التي يمكن استخدامها لحفظ الصور المُصوَّرة بصيغ TIFF أو PNG أو BMP أو JPEG"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

يُهيئ مثيلاً جديداً من الفئة [`ImageSaveOptions`](../) التي يمكن استخدامها لحفظ الصور المُصوَّرة بصيغ TIFF أو PNG أو BMP أو JPEG.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| saveFormat | SaveFileFormat | يمكن أن تكون TIFF أو PNG أو BMP أو JPEG[`SaveFileFormat`](../../savefileformat/). |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | يُرمى إذا كان *saveFormat* ليس صيغة صورة صالحة. القيم الصالحة هي TIFF أو PNG أو BMP أو JPEG. |

## الأمثلة

يوضح كيفية حفظ المشروع إلى تدفق كصورة.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // باستخدام ImageSaveOptions نحفظ المشروع بتنسيق صورة
    project.Save(stream, options);
}
```

### انظر أيضًا

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


