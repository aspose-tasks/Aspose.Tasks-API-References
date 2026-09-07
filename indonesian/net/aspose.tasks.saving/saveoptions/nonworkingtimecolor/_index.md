---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur warna waktu non-kerja"
type: docs
weight: 110
url: /id/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Mendapatkan atau mengatur warna waktu non‑kerja.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Contoh

Menampilkan cara mengatur warna khusus untuk waktu non-kerja.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### Lihat Juga

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


