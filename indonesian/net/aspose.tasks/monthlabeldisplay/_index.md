---
title: "Enum MonthLabelDisplay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.MonthLabelDisplay enum. Menentukan bagaimana label bulan ditampilkan"
type: docs
weight: 1060
url: /id/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Menentukan bagaimana label bulan ditampilkan.

```csharp
public enum MonthLabelDisplay
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Mo | `0` | Mengatur daftar Months di MS Project menjadi mo. |
| Mon | `1` | Mengatur daftar Months di MS Project menjadi mon. |
| Month | `2` | Mengatur daftar Months di MS Project menjadi month. |

## Contoh

Menampilkan cara mengatur label bulan pada opsi tampilan proyek (kasus 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// atur bagaimana label bulan ditampilkan
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


