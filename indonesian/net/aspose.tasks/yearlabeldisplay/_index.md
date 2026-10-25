---
title: "Enum YearLabelDisplay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.YearLabelDisplay enum. Menentukan bagaimana label tahun ditampilkan"
type: docs
weight: 3680
url: /id/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Menentukan bagaimana label tahun ditampilkan.

```csharp
public enum YearLabelDisplay
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Y | `0` | Mengatur daftar Years di MS Project sebagai mo. |
| Yr | `1` | Mengatur daftar Years di MS Project sebagai mon. |
| Year | `2` | Mengatur daftar Tahun di MS Project menjadi bulan. |

## Contoh

Menampilkan cara mengatur label tahun pada opsi tampilan proyek (kasus 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// atur bagaimana label tahun ditampilkan
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


