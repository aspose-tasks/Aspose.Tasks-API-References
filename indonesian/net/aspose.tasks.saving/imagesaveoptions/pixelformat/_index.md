---
title: "ImageSaveOptions.PixelFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ImageSaveOptions. Mendapatkan atau mengatur format data warna untuk setiap piksel dalam gambar"
type: docs
weight: 70
url: /id/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

Mendapatkan atau mengatur format data warna untuk setiap piksel dalam gambar.

```csharp
public PixelFormat PixelFormat { get; set; }
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


