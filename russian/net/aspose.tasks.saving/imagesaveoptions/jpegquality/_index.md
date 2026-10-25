---
title: "ImageSaveOptions.JpegQuality"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ImageSaveOptions. Получает или задает качество JPEG. Допустимый диапазон значений — 0..100"
type: docs
weight: 40
url: /ru/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Получает или задает качество JPEG. Допустимый диапазон значений — 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Примеры

Показывает, как задать качество JPEG выходных файлов.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Чтобы управлять качеством JPEG, можно использовать свойство ImageSaveOptions.JpegQuality.
// Допустимый диапазон значений: 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### См. также

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


