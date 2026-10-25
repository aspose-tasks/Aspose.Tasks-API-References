---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ImageSaveOptions. Получает или задает горизонтальное разрешение в dpi"
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Получает или задает горизонтальное разрешение в dpi.

```csharp
public float HorizontalResolution { get; set; }
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


