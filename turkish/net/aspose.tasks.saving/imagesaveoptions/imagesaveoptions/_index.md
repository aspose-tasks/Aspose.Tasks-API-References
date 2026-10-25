---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ImageSaveOptions yapıcı. Render edilen görüntüleri TIFF, PNG, BMP veya JPEG formatlarında kaydetmek için kullanılabilecek ImageSaveOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Render edilen görüntüleri TIFF, PNG, BMP veya JPEG formatlarında kaydetmek için kullanılabilecek [`ImageSaveOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | SaveFileFormat | TIFF, PNG, BMP veya JPEG[`SaveFileFormat`](../../savefileformat/) olabilir. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | *saveFormat* geçerli bir görüntü formatı değilse fırlatılır. Geçerli değerler TIFF, PNG, BMP veya JPEG'dir. |

## Örnekler

Projeyi bir akışa görüntü olarak nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // ImageSaveOptions kullanarak projeyi görüntü formatında kaydederiz
    project.Save(stream, options);
}
```

### Ayrıca Bakınız

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


