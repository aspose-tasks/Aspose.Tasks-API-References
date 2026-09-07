---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor ImageSaveOptions. Menginisialisasi instance baru dari kelas ImageSaveOptions yang dapat digunakan untuk menyimpan gambar yang dirender dalam format TIFF, PNG, BMP, atau JPEG"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Menginisialisasi instance baru dari kelas [`ImageSaveOptions`](../) yang dapat digunakan untuk menyimpan gambar yang dirender dalam format TIFF, PNG, BMP, atau JPEG.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Bisa berupa TIFF, PNG, BMP, atau JPEG[`SaveFileFormat`](../../savefileformat/). |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Dilemparkan jika *saveFormat* bukan format gambar yang valid. Nilai yang valid adalah TIFF, PNG, BMP, atau JPEG. |

## Contoh

Menampilkan cara menyimpan proyek ke dalam aliran sebagai gambar.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // dengan menggunakan ImageSaveOptions kami menyimpan proyek ke dalam format gambar
    project.Save(stream, options);
}
```

### Lihat Juga

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


