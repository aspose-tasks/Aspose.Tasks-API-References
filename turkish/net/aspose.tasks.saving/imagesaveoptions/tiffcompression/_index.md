---
title: "ImageSaveOptions.TiffCompression"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ImageSaveOptions özelliği. Oluşturulan görüntüleri TIFF formatına kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar"
type: docs
weight: 90
url: /tr/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Oluşturulan görüntüleri TIFF formatında kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Açıklamalar

Yalnızca TIFF olarak kaydederken etkili olur. Varsayılan değer `LZW`'dir.

## Örnekler

Çıktı TIFF dosyalarının TIFF sıkıştırmasını nasıl ayarlayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// TIFF sıkıştırmasını manipüle etmek için ImageSaveOptions.TiffCompression özelliğini kullanabiliriz.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### Ayrıca Bakınız

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


