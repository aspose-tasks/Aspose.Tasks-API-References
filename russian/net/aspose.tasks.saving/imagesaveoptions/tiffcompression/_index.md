---
title: "ImageSaveOptions.TiffCompression"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ImageSaveOptions. Получает или задает тип сжатия, применяемый при сохранении сгенерированных изображений в формате TIFF"
type: docs
weight: 90
url: /ru/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Получает или задает тип сжатия, применяемый при сохранении сгенерированных изображений в формате TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Примечания

Имеет эффект только при сохранении в TIFF. Значение по умолчанию — `LZW`.

## Примеры

Показывает, как установить сжатие TIFF для выходных файлов TIFF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Чтобы управлять сжатием TIFF, мы можем использовать свойство ImageSaveOptions.TiffCompression.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### См. также

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


