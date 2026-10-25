---
title: "ImageSaveOptions.JpegQuality"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعين جودة JPEG. النطاق المسموح للقيمة هو 0..100."
type: docs
weight: 40
url: /ar/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

يحصل أو يعيّن جودة JPEG. النطاق المسموح به للقيمة هو 0..100.

```csharp
public int JpegQuality { get; set; }
```

## الأمثلة

يوضح كيفية ضبط جودة JPEG لملفات JPEG الناتجة.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// من أجل تعديل جودة JPEG يمكن استخدام الخاصية ImageSaveOptions.JpegQuality.
// نطاق القيم المسموح به هو 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### انظر أيضًا

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


