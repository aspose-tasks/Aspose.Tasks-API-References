---
title: "XpsOptions.XpsOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "XpsOptions konstruktor. Menginisialisasi sebuah instance baru dari kelas XpsOptions"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Menginisialisasi sebuah instance baru dari kelas [`XpsOptions`](../).

```csharp
public XpsOptions()
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


