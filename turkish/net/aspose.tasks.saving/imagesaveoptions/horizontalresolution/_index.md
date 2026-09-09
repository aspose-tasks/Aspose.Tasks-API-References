---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ImageSaveOptions özelliği. Yatay çözünürlüğü dpi cinsinden alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Yatay çözünürlüğü dpi cinsinden alır veya ayarlar.

```csharp
public float HorizontalResolution { get; set; }
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


