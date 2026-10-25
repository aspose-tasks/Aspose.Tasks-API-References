---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ImageSaveOptions. Mendapatkan atau mengatur resolusi vertikal dalam dpi"
type: docs
weight: 100
url: /id/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Mendapatkan atau mengatur resolusi vertikal dalam dpi.

```csharp
public float VerticalResolution { get; set; }
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


