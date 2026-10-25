---
title: "ImageSaveOptions.TiffCompression"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ImageSaveOptions. Mendapatkan atau mengatur jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF"
type: docs
weight: 90
url: /id/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Mendapatkan atau mengatur jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Catatan

Berpengaruh hanya saat menyimpan ke TIFF. Nilai default adalah `LZW`.

## Contoh

Menampilkan cara mengatur kompresi TIFF pada file TIFF output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Untuk memanipulasi kompresi TIFF, kita dapat menggunakan properti ImageSaveOptions.TiffCompression.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### Lihat Juga

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


