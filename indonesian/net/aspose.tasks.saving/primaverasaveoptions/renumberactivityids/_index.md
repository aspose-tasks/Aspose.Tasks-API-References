---
title: "PrimaveraSaveOptions.RenumberActivityIds"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah perlu melakukan penomoran ulang ID aktivitas"
type: docs
weight: 50
url: /id/net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

Mendapatkan atau mengatur nilai yang menunjukkan apakah perlu menomori ulang ID aktivitas.

```csharp
public bool RenumberActivityIds { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// buat opsi penyimpanan Primavera dan sesuaikan
var options = new PrimaveraSaveOptions
                  {
                      // tentukan awalan dan akhiran sebuah aktivitas
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // kontrol penomoran ulang aktivitas
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Lihat Juga

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


