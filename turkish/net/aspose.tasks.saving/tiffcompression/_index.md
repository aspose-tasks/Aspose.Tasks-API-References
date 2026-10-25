---
title: "Enum TiffCompression"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.TiffCompression enum. Sayfaları TIFF formatında kaydederken uygulanacak sıkıştırma türünü belirtir"
type: docs
weight: 2250
url: /tr/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Sayfaları TIFF formatına kaydederken uygulanacak sıkıştırma türünü belirtir.

```csharp
public enum TiffCompression
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `1` | Sıkıştırma olmadığını belirtir. |
| Rle | `2` | RLE sıkıştırma şemasını belirtir. |
| Ccitt3 | `3` | CCITT3 sıkıştırma şemasını belirtir. |
| Ccitt4 | `4` | CCITT4 sıkıştırma şemasını belirtir. |
| Lzw | `5` | LZW sıkıştırma şemasını belirtir. |

## Örnekler

RLE sıkıştırma modunu kullanarak TIFF formatında nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Projeyi RLE sıkıştırmasıyla kaydedin
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


