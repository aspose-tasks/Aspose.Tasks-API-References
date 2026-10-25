---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ImageSaveOptions. Получает или задает вертикальное разрешение в dpi."
type: docs
weight: 100
url: /ru/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Получает или задает вертикальное разрешение в dpi.

```csharp
public float VerticalResolution { get; set; }
```

## Примеры

Показывает, как задать формат пикселей, используемый при конвертации в форматы изображений.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### См. также

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


