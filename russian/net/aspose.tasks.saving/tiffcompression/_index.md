---
title: "Enum TiffCompression"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.TiffCompression enum. Указывает, какой тип сжатия применять при сохранении страниц в формате TIFF"
type: docs
weight: 2250
url: /ru/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Указывает, какой тип сжатия применять при сохранении страниц в формате TIFF.

```csharp
public enum TiffCompression
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `1` | Указывает отсутствие сжатия. |
| Rle | `2` | Указывает схему сжатия RLE. |
| Ccitt3 | `3` | Указывает схему сжатия CCITT3. |
| Ccitt4 | `4` | Указывает схему сжатия CCITT4. |
| Lzw | `5` | Указывает схему сжатия LZW. |

## Примеры

Показывает, как отрисовать в формате TIFF, используя режим сжатия RLE.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Сохранить проект с сжатием Rle
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### См. также

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


