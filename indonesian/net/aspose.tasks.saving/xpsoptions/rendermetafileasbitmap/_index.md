---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti XpsOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah metafile harus dirender sebagai bitmap."
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Mendapatkan atau mengatur nilai yang menunjukkan apakah metafile harus dirender sebagai bitmap.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## Contoh

Menampilkan cara menyimpan proyek sebagai file XPS.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// buat opsi penyimpanan XPS dan sesuaikan parameter
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### Lihat Juga

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


