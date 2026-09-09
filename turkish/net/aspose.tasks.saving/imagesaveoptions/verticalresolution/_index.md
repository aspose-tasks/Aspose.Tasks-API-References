---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ImageSaveOptions özelliği. Dikey çözünürlüğü dpi cinsinden alır veya ayarlar"
type: docs
weight: 100
url: /tr/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Dikey çözünürlüğü dpi cinsinden alır veya ayarlar.

```csharp
public float VerticalResolution { get; set; }
```

## Örnekler

Görüntü formatlarına dönüşüm sırasında kullanılan piksel biçiminin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### Ayrıca Bakınız

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


