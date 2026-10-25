---
title: "Enum TiffCompression"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.TiffCompression. Menentukan jenis kompresi yang diterapkan saat menyimpan halaman ke format TIFF"
type: docs
weight: 2250
url: /id/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Menentukan jenis kompresi yang diterapkan saat menyimpan halaman ke format TIFF.

```csharp
public enum TiffCompression
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `1` | Menentukan tidak ada kompresi. |
| Rle | `2` | Menentukan skema kompresi RLE. |
| Ccitt3 | `3` | Menentukan skema kompresi CCITT3. |
| Ccitt4 | `4` | Menentukan skema kompresi CCITT4. |
| Lzw | `5` | Menentukan skema kompresi LZW. |

## Contoh

Menampilkan cara merender dalam format TIFF dengan menggunakan mode kompresi RLE.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Simpan proyek dengan kompresi Rle
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### Lihat Juga

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


