---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ImageSaveOptions. Mendapatkan atau mengatur resolusi horizontal dalam dpi"
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Mendapatkan atau mengatur resolusi horizontal dalam dpi.

```csharp
public float HorizontalResolution { get; set; }
```

## Contoh

Menampilkan cara mengatur format piksel yang digunakan selama konversi ke format gambar.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### Lihat Juga

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


