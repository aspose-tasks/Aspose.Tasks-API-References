---
title: "ImageSaveOptions.JpegQuality"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ImageSaveOptions özelliği. JPEG kalitesini alır veya ayarlar. İzin verilen değer aralığı 0..100'tür."
type: docs
weight: 40
url: /tr/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

JPEG kalitesini alır veya ayarlar. İzin verilen değer aralığı 0..100'dür.

```csharp
public int JpegQuality { get; set; }
```

## Örnekler

Çıktı JPEG dosyalarının JPEG kalitesini nasıl ayarlayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// JPEG kalitesini değiştirmek için ImageSaveOptions.JpegQuality özelliğini kullanabilirsiniz.
// İzin verilen değer aralığı 0..100'tür.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### Ayrıca Bakınız

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


