---
title: "ImageSaveOptions.JpegQuality"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ImageSaveOptions. Mendapatkan atau mengatur kualitas JPEG. Rentang nilai yang diizinkan adalah 0..100"
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Mendapatkan atau mengatur kualitas JPEG. Rentang nilai yang diizinkan adalah 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Contoh

Menampilkan cara mengatur kualitas JPEG pada file JPEG keluaran.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Untuk memanipulasi kualitas JPEG, dapat menggunakan properti ImageSaveOptions.JpegQuality.
// Rentang nilai yang diizinkan adalah 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### Lihat Juga

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


